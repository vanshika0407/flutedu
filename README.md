# flutedu


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign Up and Browse Courses</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            margin: 0;
        }

        .signup-form-container, .browse-courses-container {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            display: flex;
            max-width: 900px;
            width: 100%;
            margin: 20px 0;
        }

        .profile-info,
        .form-background {
            background-image: url('https://cdn.pixabay.com/photo/2017/08/06/22/01/books-2596809_1280.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
        }

        .profile-info {
            color: white;
            padding: 20px;
            text-align: center;
            width: 30%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .profile-info img {
            border-radius: 50%;
            width: 100px;
            height: 100px;
        }

        .profile-info h2 {
            margin: 10px 0;
        }

        .profile-info .availability {
            color: #2ecc71;
        }

        .form-background {
            position: relative;
            width: 70%;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }

        .background-img {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: 1;
        }

        .form-content {
            position: relative;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 10px;
            padding: 40px;
            z-index: 2;
            display: flex;
            align-items: center;
        }

        .sitting-girl {
            width: 100px;
            margin-right: 20px;
        }

        .signup-form, .browse-courses {
            width: 100%;
        }

        .signup-form h1, .browse-courses h1 {
            margin-bottom: 20px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
        }

        .form-group input, .form-group select {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        button {
            background-color: #2c3e50;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #34495e;
        }

        .country-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            padding: 20px;
        }

        .country-box {
            position: relative;
            width: 200px;
            height: 150px;
            cursor: pointer;
        }

        .country-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .overlay {
            position: absolute;
            bottom: 0;
            background: rgba(0, 0, 0, 0.5);
            color: #fff;
            width: 100%;
            text-align: center;
            padding: 10px 0;
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            background: #fff;
            padding: 20px;
            border-radius: 5px;
            max-width: 800px;
            width: 90%;
            max-height: 90%;
            overflow-y: auto;
        }

        .close {
            position: absolute;
            top: 10px;
            right: 20px;
            font-size: 24px;
            cursor: pointer;
        }

        .courses-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .course-box {
            position: relative;
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            margin-bottom: 10px;
        }

        .course-box img {
            width: 50px;
            height: 50px;
            object-fit: cover;
            float: left;
            margin-right: 10px;
        }

        .course-details {
            overflow: hidden;
        }

       #client feedback-container
       font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}



        }
        .feedback-container {
    width: 80%;
    margin: 0 auto;
    padding: 20px;
    text-align: center;
 flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 0;
}

h2 {
    margin-bottom: 20px;
 text-align: center;
}

.feedback {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.feedback-item {
    background: #f9f9f9;
    border: 1px solid #ddd;
    border-radius: 5px;
    padding: 20px;
    margin: 10px;
    width: 30%;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
 text-align: center;
}

.feedback-item img {
    max-width: 50%;
    height: auto;
}

.feedback-item p {
    font-size: 14px;
    line-height: 1.5;
}

.feedback-item .author {
    font-weight: bold;
    margin-top: 10px;
} 

        .footer {
            background-color: #089592;
            color: white;
            padding: 20px;
            text-align: center;
            width: 100%;
            box-sizing: border-box;
        }
        .footer a {
            color: white;
            text-decoration: none;
            display: block;
            margin: 5px 0;
        }
        .footer a:hover {
            text-decoration: underline;
        }
        .footer .feedback {
            margin-top: 20px;
        }
        .footer .feedback textarea {
            padding: 10px;
            width: 70%;
            margin-right: 10px;
            resize: vertical;
        }
        .footer .feedback input[type="submit"] {
            padding: 10px;
            border: none;
            background-color: black;
            color: white;
            cursor: pointer;
        }
        .feedback-chatbox {
            position: fixed;
            bottom: 10px;
            right: 10px;
            background-color: black;
            border: 1px solid #ccc;
            padding: 10px;
            width: 300px;
            box-shadow: 0 10px 10px rgba(0, 0, 0, 0.1);
        }
        .feedback-chatbox h2 {
            margin: 0 0 10px;
        }
        .feedback-chatbox textarea {
            width: 100%;
            height: 1000px;
            margin-bottom: 10px;
        }
        .feedback-chatbox input[type="submit"] {
            padding: 10px;
            border: none;
            background-color: #009688;
            color: white;
            cursor: pointer;
            width: 100%;
        }


footer {
    background-color: #089592; /* Black background */
    padding: 20px 0;
    text-align: center;
}

.social-icons a {
    text-decoration: none;
    margin: 0 10px;
    display: inline-block;
}

.social-icons img {
    width: 40px;  /* Adjust the size of the icons as needed */
    height: 40px;
    border: 2px solid #fff; /* White border */
    border-radius: 50%;
    padding: 5px;
    background-color: #000; /* Black background */
}

.social-icons a:hover img {
    background-color: #fff; /* White background on hover */
    border-color: #000; /* Black border on hover */
}
 .error {
        color: red;
        font-size: 14px;
    }
.countdown-box {
            display: none;
            margin-top: 20px;
            font-size: 20px;
            font-weight: bold;
        }
        .chatbox-message {
            display: none;
            margin-top: 20px;
            font-size: 20px;
            font-weight: bold;
            color: red;
        }


 


    </style>
</head>
<body>
    <div class="signup-form-container">
        <div class="profile-info">
            <img src="https://i.pinimg.com/originals/d6/23/93/d623934e162324219c99e435162f1158.jpg" alt="Profile Picture">
            <h2>Flutedu</h2>
            <p class="availability"></p>
        </div>
        <div class="form-background">
            <div class="form-content">
                <img src="https://img.freepik.com/premium-photo/girl-with-book-her-lap-is-sitting-library-books_662214-67065.jpg?w=360" alt="Sitting Girl" class="sitting-girl">
                <div class="signup-form">
                    <h1>Sign Up Form</h1>
                    <form id="signup-form" onsubmit="startCountdown(event)">
                        <div class="form-group">
                            <label for="name">Your Name</label>
                            <input type="text" id="name" name="name" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Your Email</label>
                            <input type="email" id="email" name="email" required>
                        </div>
                        <div class="form-group">
                            <label for="country">Country</label>
                            <select id="country" name="country" required>
                                <option value="" disabled selected>Select an option</option>
                                <option value="India">India</option>
                                <option value="US">US</option>
                                <option value="UK">UK</option>
                                <option value="Belgium">Belgium</option>
                                <option value="Korea">Korea</option>
                                <option value="Australia">Australia</option>
                                <option value="Canada">Canada</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="phone">Phone Number</label>
                            <input type="tel" id="phone" name="phone" required pattern="[0-9]{10}" oninput="validatePhone(this);">
                            <span class="error">Please enter a 10-digit phone number.</span>
                        </div>
                        <div class="form-group">
                            <label for="help">Help to find</label>
                            <select id="help" name="help" required>
                                <option value="" disabled selected>Select an option</option>
                                <option value="University">University</option>
                                <option value="Course">Course</option>
                            </select>
                        </div>
                        <button type="submit">Submit</button>
                    </form>
                    <div class="countdown-box" id="countdown-box">
                        <p>Time remaining: <span id="countdown-timer">6</span> seconds</p>
                    </div>
                    <div class="chatbox-message" id="chatbox-message">
                        <p>Click on the chatbox ---></p>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div id="browse-courses-container" class="browse-courses-container" style="display: none;">
        <h1>Browse by Country</h1>
        <div class="country-grid">
            <div class="country-box" onclick="showCourseForm('India')">
                <img src="https://static.dw.com/image/62272669_605.jpg" alt="India">
                <div class="overlay">India</div>
            </div>
            <div class="country-box" onclick="showCourseForm('USA')">
                <img src="https://ichef.bbci.co.uk/news/976/cpsprodpb/360D/production/_86373831_nymidtownskyline_2012_getty.jpg" alt="USA">
                <div class="overlay">USA</div>
            </div>
            <div class="country-box" onclick="showCourseForm('UK')">
                <img src="https://www.nationsonline.org/gallery/UK/Palace-of-Westminster-Parliament.jpg" alt="UK">
                <div class="overlay">UK</div>
            </div>
            <div class="country-box" onclick="showCourseForm('Australia')">
                <img src="https://www.umultirank.org/export/sites/default/.galleries/generic-images/Others/Winter-Calendar/why-should-I-study-in-Sydney.jpg_1079324579.jpg" alt="Australia">
                <div class="overlay">Australia</div>
            </div>
            <div class="country-box" onclick="showCourseForm('Korea')">
                <img src="https://www.nationsonline.org/gallery/Korea_South/Seoul-Seongsan-Bridge-and-the-Han-River.jpg" alt="Korea">
                <div class="overlay">Korea</div>
            </div>
            <div class="country-box" onclick="showCourseForm('Canada')">
                <img src="https://www.vmcdn.ca/f/files/via/import/2018/08/28153211_vancouver_skyline.jpg;w=960" alt="Canada">
                <div class="overlay">Canada</div>
            </div>
            <div class="country-box" onclick="showCourseForm('Belgium')">
                <img src="https://media.istockphoto.com/id/476653220/photo/ghent.jpg?s=612x612&w=0&k=20&c=a2Adwd1lH4Vd27MB82cMHzb59gBNxQtccX8aFtTdoNg=" alt="Belgium">
                <div class="overlay">Belgium</div>
            </div>
        </div>

        <div id="course-form-modal" class="modal">
            <div class="modal-content">
                <span class="close" onclick="closeModal()">&times;</span>
                <h2 id="form-country-name"></h2>
                <form id="course-form">
                    <label for="course-select">Choose a course:</label>
                    <select id="course-select" name="course">
                        <option value="" disabled selected>Select an option</option>
                        <option value="BCA">BCA</option>
<option value="BTech(Computer science and engineering)">BTech(Computer science and engineering)</option>
                                      <option value="BTech(Mechanical engineering)">BTech(Mechanical engineering)</option>
                                      <option value="BTech(Civil engineering)">BTech(Civil engineering)</option>
                                      <option value="BTech(Eloctronics &computer engineering)">BTech(Eloctronics & communication engineering)</option>
                                      <option value="BTech(Electrical engineering)">BTech(Electrical engineering)</option>
                                      <option value="BTech(Aeronautical engineering)">BTech(Aeronautical engineering)</option>
                                      <option value="BTech(Biotechnology engineering)">BTech(Biotechnology engineering)</option>
                                      <option value="BTech(Automobile engineering)">BTech(Automobile engineering)</option>

                       <option value="BBA">BBA</option>

                      <option value="B.Com(Computer application)">B.Com(Computer application)</option>
                                       <option value="B.Com(Hons.)">B.Com(Hons.)</option>
                                       <option value="B.Com(Accounting and Finance)">B.Com(Accounting and Finance)</option>
                                       <option value="B.Com(Corporate Secretaryship)">B.Com(Corporate Secretaryship)</option>
                                       <option value="B.Com(Banking and insurance)">B.Com(Banking and insurance)</option>


                      <option value="B.ED(Hindi)">B.ED(Hindi)</option>
                                       <option value="B.ED(Computer science)">B.ED(Computer science)</option>
                                       <option value="B.ED(Sanskrit)">B.ED(Sanskrit)</option>
                                       <option value="B.ED(English)">B.ED(English)</option>
                                       <option value="B.ED(Commerce)">B.ED(Commerce)</option>
                                       <option value="B.ED(Physical science)">B.ED(Physical science)</option>
                                       <option value="B.ED(Psychology)">B.ED(Psychology)</option>
                                       <option value="B.ED(Physical science)">B.ED(Physical science)</option>
                                       <option value="B.ED(Economics)">B.ED(Economics)</option>
                                      <option value="B.ED(Mathematics)">B.ED(Mathematics)</option>

                       <option value="B.Pharm">B.Phram</option>
                       <option value="D.Phram">D.Phram</option>
                       <option value="LLB">LLB</option>
                      
                       <option value="BA">BA(English)</option>
                                       <option value="BA(Economics)">BA(Economics)</option>
                                       <option value="BA(History)">BA(History)</option>
                                       <option value="BA(Political science)">BA(Political science)</option>
                                       <option value="BA(Sociology)">BA(Sociology)</option>
                                       <option value="BA(Hindi)">BA(Hindi)</option>
                                       <option value="BA(Geography)">BA(Geography)</option>

                        <option value="Bsc(Chemistry)">Bsc(Chemistry)</option>
                                       <option value="Bsc(Biology)">Bsc(Biology)</option>
                                       <option value="Bsc(Mathematics)">Bsc(Mathematics)</option>
                                       <option value="Bsc(IT)">Bsc(IT)</option>
                                       <option value="Bsc(Computer science)">Bsc(Computer science)</option>
                                       <option value="Bsc(Biochemistry)">Bsc(Biochemistry)</option>
                                       <option value="Bsc(Botany)">Bsc(Botany)</option>
                                       <option value="Bsc(Zoology)">Bsc(Zoology)</option>
                                       <option value="Bsc(Agriculture)">Bsc(Agriculture)</option>
                                       <option value="Bsc(Fashion design)">Bsc(Fashion design)</option>
                                       <option value="Bsc(Animation)">Bsc(Animation)</option>
                                       <option value="Bsc(Geography)">Bsc(Geography)</option>
                                       <option value="Bsc(Economics)">Bsc(Economics)</option>
                                       <option value="Bsc(Nursing)">Bsc(Nursing)</option>

                            <option value="MA">MA(English)</option>
                                       <option value="MA(Economics)">MA(Economics)</option>
                                       <option value="MA(History)">MA(History)</option>
                                       <option value="MA(Political science)">MA(Political science)</option>
                                       <option value="MA(Sociology)">MA(Sociology)</option>
                                       <option value="MA(Hindi)">MA(Hindi)</option>
                                       <option value="MA(Geography)">MA(Geography)</option>

                            <option value="MBA">MBA</option>
                            <option value="Mtech">Mtech</option>
                            <option value="MCA">MCA</option>

                            <option value="M.ED(Hindi)">M.ED(Hindi)</option>
                                       <option value="M.ED(Computer science)">M.ED(Computer science)</option>
                                       <option value="M.ED(Sanskrit)">M.ED(Sanskrit)</option>
                                       <option value="M.ED(English)">M.ED(English)</option>
                                       <option value="M.ED(Commerce)">M.ED(Commerce)</option>
                                       <option value="M.ED(Physical science)">M.ED(Physical science)</option>
                                       <option value="M.ED(Psychology)">M.ED(Psychology)</option>
                                       <option value="M.ED(Physical science)">M.ED(Physical science)</option>
                                       <option value="M.ED(Economics)">M.ED(Economics)</option>
                                      <option value="M.ED(Mathematics)">M.ED(Mathematics)</option>

                             <option value="M.Com(Computer application)">M.Com(Computer application)</option>
                                       <option value="M.Com(Hons.)">M.Com(Hons.)</option>
                                       <option value="M.Com(Accounting and Finance)">M.Com(Accounting and Finance)</option>
                                       <option value="M.Com(Corporate Secretaryship)">M.Com(Corporate Secretaryship)</option>
                                       <option value="M.Com(Banking and insurance)">M.Com(Banking and insurance)</option>

                             <option value="Msc(Chemistry)">Msc(Chemistry)</option>
                                       <option value="Msc(Biology)">Msc(Biology)</option>
                                       <option value="Msc(Mathematics)">Msc(Mathematics)</option>
                                       <option value="Msc(IT)">Msc(IT)</option>
                                       <option value="Msc(Computer science)">Msc(Computer science)</option>
                                       <option value="Msc(Biochemistry)">Msc(Biochemistry)</option>
                                       <option value="Msc(Botany)">Msc(Botany)</option>
                                       <option value="Msc(Zoology)">Msc(Zoology)</option>
                                       <option value="Msc(Agriculture)">Msc(Agriculture)</option>
                                       <option value="Msc(Fashion design)">Msc(Fashion design)</option>
                                       <option value="Msc(Animation)">Msc(Animation)</option>
                                       <option value="Msc(Geography)">Msc(Geography)</option>
                                       <option value="Msc(Economics)">Msc(Economics)</option>
                                       <option value="Msc(Nursing)">Msc(Nursing)</option>




                    </select>
                    <button type="submit">Submit</button>
                </form>
            </div>
        </div>


        <div id="courses-modal" class="modal">
            <div class="modal-content">
                <span class="close" onclick="closeModal()">&times;</span>
                <h2 id="country-name"></h2>
                <div id="courses-grid" class="courses-grid"></div>
            </div>
        </div>
    </div>
    <script>
        document.getElementById('help').addEventListener('change', function() {
            if (this.value === 'Course') {
                !function() {
                    var t = window.driftt = window.drift = window.driftt || [];
                    if (!t.init) {
                        if (t.invoked) return void (window.console && console.error && console.error("Drift snippet included twice."));
                        t.invoked = !0, t.methods = ["identify", "config", "track", "reset", "debug", "show", "ping", "page", "hide", "off", "on"],
                        t.factory = function(e) {
                            return function() {
                                var n = Array.prototype.slice.call(arguments);
                                return n.unshift(e), t.push(n), t;
                            };
                        }, t.methods.forEach(function(e) {
                            t[e] = t.factory(e);
                        }), t.load = function(t) {
                            var e = 3e5, n = Math.ceil(new Date() / e) * e, o = document.createElement("script");
                            o.type = "text/javascript", o.async = !0, o.crossorigin = "anonymous", o.src = "https://js.driftt.com/include/" + n + "/" + t + ".js";
                            var i = document.getElementsByTagName("script")[0];
                            i.parentNode.insertBefore(o, i);
                        };
                    }
                }();
                drift.SNIPPET_VERSION = '0.3.1';
                drift.load('shvhvsxbehcy');
            }
        });

        function startCountdown(event) {
            event.preventDefault(); // Prevent the form from submitting immediately

            var countdownBox = document.getElementById('countdown-box');
            var countdownTimer = document.getElementById('countdown-timer');
            var chatboxMessage = document.getElementById('chatbox-message');
            var timeLeft = 6;

            countdownBox.style.display = 'block';
            countdownTimer.textContent = timeLeft;

            var countdownInterval = setInterval(function() {
                timeLeft--;
                countdownTimer.textContent = timeLeft;

                if (timeLeft <= 0) {
                    clearInterval(countdownInterval);
                    countdownBox.style.display = 'none';
                    chatboxMessage.style.display = 'block'; // Display the chatbox message
                }
            }, 1000);
        }

        function validatePhone(input) {
            // Phone validation logic here
        }

        function showCourseForm(country) {
            // Show course form for selected country
        }

        function closeModal() {
            // Close modal logic
        }
    </script>


        <div id="courses-modal" class="modal">
            <div class="modal-content">
                <span class="close" onclick="closeModal()">&times;</span>
                <h2 id="country-name"></h2>
                <div id="courses-grid" class="courses-grid"></div>
            </div>
        </div>
    </div>

    <script>
        document.getElementById('signup-form').addEventListener('submit', function(event) {
            event.preventDefault();
            const helpValue = document.getElementById('help').value;
            if (helpValue === 'University') {
                document.querySelector('.signup-form-container').style.display = 'none';
                document.getElementById('browse-courses-container').style.display = 'block';
            } else {
                alert('Form submitted successfully.');
            }
        });

        function showCourseForm(country) {
            document.getElementById('form-country-name').innerText = country;
            document.getElementById('course-form').dataset.country = country;
            document.getElementById('course-form-modal').style.display = 'flex';
        }

        function closeModal() {
            document.getElementById('course-form-modal').style.display = 'none';
            document.getElementById('courses-modal').style.display = 'none';
        }

        document.getElementById('course-form').addEventListener('submit', function(event) {
            event.preventDefault();
            const country = event.target.dataset.country;
            const course = document.getElementById('course-select').value;
            showCourseDetails(country, course);
        });

        function showCourseDetails(country, course) {
            document.getElementById('country-name').innerText = `${country} - ${course}`;
            const coursesGrid = document.getElementById('courses-grid');
            coursesGrid.innerHTML = '';

            const courses = {
                'India': {
                    'BCA': [
                        {name: 'Christ University', placement: '90%', fees: '₹6.60 Lakh', image: 'christ.jpg', location: 'Bangalore'},
                        {name: 'St. Joseph\'s University', placement: '85%', fees: '₹3.00 Lakh', image: 'st_joseph.jpg', location: 'Bangalore'}
                    ],
                    'BTech': [
                        {name: 'IIT Bombay', placement: '95%', fees: '₹8.00 Lakh', image: 'iit_bombay.jpg', location: 'Mumbai'},
                        {name: 'NIT Trichy', placement: '92%', fees: '₹5.50 Lakh', image: 'nit_trichy.jpg', location: 'Tiruchirappalli'}
                    ],
                },
                'USA': {
                    'BSc': [
                        {name: 'Harvard University', placement: '98%', fees: '$50,000', image: 'harvard.jpg', location: 'Cambridge'},
                        {name: 'Stanford University', placement: '97%', fees: '$55,000', image: 'stanford.jpg', location: 'Stanford'}
                    ],
                    'BBA': [
                        {name: 'Wharton School', placement: '95%', fees: '$60,000', image: 'wharton.jpg', location: 'Philadelphia'},
                        {name: 'MIT Sloan', placement: '96%', fees: '$58,000', image: 'mit_sloan.jpg', location: 'Cambridge'}
                    ],
                }
            };

            if (courses[country] && courses[country][course]) {
                courses[country][course].forEach(courseDetail => {
                    const courseBox = document.createElement('div');
                    courseBox.className = 'course-box';
                    courseBox.innerHTML = `
                        <img src="${courseDetail.image}" alt="${courseDetail.name}">
                        <div class="course-details">
                            <h3>${courseDetail.name}</h3>
                            <p>Placement: ${courseDetail.placement}</p>
                            <p>Fees: ${courseDetail.fees}</p>
                            <p>Location: ${courseDetail.location}</p>
                        </div>
                    `;
                    coursesGrid.appendChild(courseBox);
                });
            } else {
                coursesGrid.innerHTML = '<p>No courses available for the selected option.</p>';
            }

            document.getElementById('course-form-modal').style.display = 'none';
            document.getElementById('courses-modal').style.display = 'flex';
        }
    </script>
<br>

<div class="feedback-container">
               <div class="feedback">
            <div class="feedback-item">
                <img src="C:\Users\ritik\OneDrive\Pictures\Screenshots\Screenshot 2024-05-29 120418.png" alt="VIT University">
                <p>"I can't express how much this website has simplified my university search process. The user-friendly interface and comprehensive filters allowed me to find the perfect courses tailored to my interests and career goals. The student reviews and ratings were incredibly insightful and helped me make an informed decision. Thank you for making such a stressful process so much easier!"</p>
                <p class="author">Ritik nehra,<br>Student if VIT University(India)</p>
            </div>

            <div class="feedback-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR4VXUNs5iK8jbN-PsyqDcNoqML3pVOtoSR3A&s" alt="Harvard University">
               <p>"This website is a game-changer for anyone looking to find the right university and courses. The detailed information and extensive database made it easy to compare different options. I particularly loved the personalized recommendations and the real-life student experiences shared here. It's like having a mentor guide you through the entire process. Highly recommended!"</p>
                <p class="author">John F. Kennedy,<br>Sudent of Harvard University(US) </p>
            </div>

            <div class="feedback-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTtf-73dWDUzOJgKC_m8cAuFugzhRDT6-lC9A&s" alt="The Australia National University">
                <p>"Finding the right course and university was daunting until I discovered this website. The layout is intuitive, and the search functionality is top-notch. What sets this site apart is the wealth of firsthand reviews from current students, which provided valuable insights that brochures and official websites often miss. Thanks to this platform, I feel confident and excited about my academic future!"
</p>
                <p class="author">Hayes,<br>Student of The Australia National University(Australia)</p>
            </div>

<div class="feedback-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTawxYOWxeOPdnY5euBsuQdMYTrpiLUj0usGw&s" alt="Seoul National University">
                <p>"This website has been an invaluable resource during my university search. The detailed course descriptions and up-to-date information on each institution made it easy to compare my options. I particularly appreciated the honest feedback from other students, which gave me a clearer picture of what to expect. It’s a must-visit for anyone serious about their education."</p>
                <p class="author">Hwa Young,<br>Sudent of Seoul National University(Korea) </p>
            </div>

<div class="feedback-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRuwYj1aBgf3YVfeBKx1hNFFB4Sgd9GOIbcLw&s" alt="University of Alberta">
                <p>"I’m so grateful for this website! It took the guesswork out of finding the right university and courses for me. The search tools are precise and saved me so much time. Reading reviews and tips from fellow students gave me a sense of community and support. This site turned my overwhelming search into an enjoyable experience. I couldn't be happier with the results!"
</p>
                <p class="author">Mia,<br>Sudent of University of Alberta(Canada) </p>
            </div>


        </div>
    </div>
<div class="footer">
    <div>
        <a href="#">Terms Of Service</a>
        <a href="#">Privacy Policy</a>
    </div>
    <div>
        <a href="https://www.instagram.com/flutedu_07?utm_source=qr&igsh=MTB4ZTIrbno5amVrMw==">Contact Us</a>
        <a href="#">About Us</a>
        <a href="#">Security</a>
    </div>
    <div class="feedback">
        <form action="connect.php" method="post">
            <textarea name="feedback" placeholder="Enter your feedback here"></textarea>
            <input type="submit" value="Submit">
        </form>
    </div>
    <footer>
        <div class="social-icons">
            <a href="https://www.instagram.com/flutedu_07?utm_source=qr&igsh=MTB4ZTIrbno5amVrMw==" target="_blank"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRwH--J-ZMUg8puNfUxE6YXQi3yVHuAORDxow&s" ></a>
            <a href="https://www.facebook.com/profile.php?id=61560880169482&mibextid=ZbWKwL" target="_blank"><img src="https://www.freepnglogos.com/uploads/logo-facebook-png/logo-facebook-facebook-logo-transparent-png-pictures-icons-and-0.png" ></a>
            <a href="https://x.com/flutedu07?t=S76xoPuG-5cXFowmQf1Lnw&s=09" target="_blank"><img src="https://cdn.pixabay.com/photo/2017/08/23/11/30/twitter-2672572_1280.jpg" ></a>
                       <a href="https://www.youtube.com/@flutedu07" target="_blank"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS0vjqOGyOmZ4N4Atj0Wrujl7yP-_2iMDxzTg&s" ></a>
            <a href="https://www.pinterest.com/flutedu07" target="_blank"><img src="https://static-00.iconduck.com/assets.00/pinterest-icon-2048x2048-d7p0u7c5.png" ></a>
        </div>
    </footer>

    <!-- Add Font Awesome CDN link -->
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
    <div>
        <p>&copy; 2024 Flutedu</p>
    </div>
</div>



</body>
</html>

