        main {
            padding: 20px;
            text-align: left;
            max-width: 800px;
            margin: 0 auto;
        }

        section {
            margin-bottom: 20px;
        }

        h2 {
            cursor: pointer;
            background-color: #f0f0f0;
            padding: 10px;
            margin: 0;
        }

        p {
            margin-top: 0;
        }

        .content {
            display: none;
            padding: 10px;
        }

        .active {
            display: block;
        }
    </style>
</head>
<body>

    <header>
        <h1>Your Name</h1>
    </header>

    <main>
        <section id="about">
            <h2>About Me</h2>
            <div class="content">
                <p>I am a passionate and driven individual with a strong desire to pursue a career in [your field of study]. I was born and raised in [your hometown], where I developed a love for [your interests].</p>
                <p>Throughout my academic journey, I have consistently challenged myself and achieved success in various subjects, particularly [mention specific subjects or areas of interest].</p>
            </div>
        </section>

        <section id="achievements">
            <h2>Achievements</h2>
            <div class="content">
                <ul>
                    <li>Recipient of the [Name of Scholarship/Award]</li>
                    <li>Member of the National Honor Society</li>
                    <li>AP Scholar with Distinction</li>
                    <!-- Add more achievements as needed -->
                </ul>
            </div>
        </section>

        <section id="extracurricular">
            <h2>Extracurricular Activities</h2>
            <div class="content">
                <ul>
                    <li>President of the Science Club</li>
                    <li>Captain of the Varsity Soccer Team</li>
                    <li>Volunteer at [Organization/Event]</li>
                    <!-- Add more extracurricular activities as needed -->
                </ul>
            </div>
        </section>

        <section id="goals">
            <h2>Career Goals</h2>
            <div class="content">
                <p>My ultimate career goal is to [describe your long-term career goal]. I am particularly interested in [specific aspect of your field], and I aspire to [describe how you plan to make a positive impact in your field].</p>
            </div>
        </section>
    </main>

    <footer>
        <p>Contact: your@email.com | Phone: (123) 456-7890</p>
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            var sections = document.querySelectorAll('section');

            sections.forEach(function(section) {
                var header = section.querySelector('h2');

                header.addEventListener('click', function() {
                    sections.forEach(function(s) {
                        if (s !== section) {
                            s.querySelector('.content').classList.remove('active');
                        }
                    });

                    section.querySelector('.content').classList.toggle('active');
                });
            });
        });
    </script>

</body>
</html>
