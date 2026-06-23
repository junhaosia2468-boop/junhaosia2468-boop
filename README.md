## Hi there 👽

I'm Nicholas, a developer based in Singapore.

I design and build whatever I can imagine.

If an idea pops into my head, chances are I'll build it and ship it.

My main tech stack is Python, WordPress, and Elementor. My favorite tools are Blender, Figma, and Google Ads.

I've got a bunch of pinned projects, but my favorite is currently [Insert Name of your favorite project here].

I'm constantly working on new public repos to sharpen my skills.

If you want to see what I’m building, check out my repositories below!

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="{{ url_for('static', filename='index.css') }}">
    <link rel="stylesheet" href="{{url_for('static', filename='style.css')}}">
    <title>Nicholas project</title>
</head>
<body>
    <header>
        <p>Website For EAE :<</p>
    </header>

    <nav>
        <div class="navigation">
            <hr>
            <ul>
                <li><a href="/">Home</a></li>
                <li><a href="/news">News</a></li>
                <li><a href="">About Us</a></li>
                <li><a href="">Contact Us</a></li>
            </ul>
            <hr>
        </div>
    </nav>

    <div class="main-content">
        <main class="picture1">
            <img src="{{ url_for('static', filename='picture/main1.jpg')}}" alt="main">
        </main>

        <div class="sidebar-top">
            <h3>In-Depth Analysis</h3>
            <p>
                As urban traffic density continues to climb, the critical issue of night-time road safety has once again moved to the forefront of municipal policy. Recent data suggests that over 60% of major accidents occur under low-light conditions, where human reaction times are significantly hampered by reduced visibility. 
            </p>
            <p>
                Transportation experts argue that simply installing more streetlights is no longer a sufficient solution. Instead, they are calling for a multi-layered approach: integrating smart, sensor-driven vehicle lighting systems with infrastructure-linked warning signals. Such technology could potentially bridge the gap between human perception and real-time hazards, offering a much-needed layer of protection for drivers and pedestrians alike in our increasingly busy urban environments.
            </p>
            <a href="#" style="color: #c0392b; font-weight: bold; text-decoration: none;">Read Full Report ></a>
        </div>

        <div class="sidebar-down">
            <h3>Flash Updates</h3>
            <ul>
                <li><strong>[10:45 AM]</strong> Municipal Department: South Ring Road to be closed for maintenance tomorrow.</li>
                <li><strong>[09:20 AM]</strong> Meteorological Office: Yellow alert issued for heavy fog tonight.</li>
                <li><strong>[08:00 AM]</strong> Transport Authority: Crackdown on illegal parking and unlit vehicles begins today.</li>
            </ul>
        </div>
    </div>

    <h1 class="mainly">Some other news that also popular</h1>

    <div class="second-contain">
        <div class="sc_pic_1">
            <img src="{{ url_for('static', filename='picture/content1.jpg')}}" alt="content1">
            <h4>Why Communication Fails: Stop the Cycle of Argumentation</h4>
            <p>Arguments are not merely disagreements; they are destructive feedback loops that drain our mental clarity and erode the foundation of productive cooperation. When we choose to engage in aggressive rhetoric, we prioritize "winning" over "understanding." This reactive behavior triggers a physiological stress 
                response that clouds judgment and shuts down empathy. We must transition from reactive noise to active listening. True communication is not about overpowering the other side; it is
                 about finding a common ground where logical problem-solving can occur. Next time you feel the urge to retort, ask yourself: is this for progress, or merely for ego? Silence is often the most sophisticated tool in your arsenal to de-escalate tension and restore order.</p>
        </div>
        <div class="sc_pic_2">
            <img src="{{ url_for('static', filename='picture/content2.jpg')}}" alt="content1">
            <h4>Discipline: The Only Bridge Between Goals and Accomplishment</h4>
            <p>Discipline is often misidentified as a form of self-punishment, when in reality, it is the ultimate form of self-respect. Motivation is a volatile, fleeting chemical surge in the brain—it cannot be relied upon to build anything of 
                lasting significance. Discipline, however, is a persistent habit built on the refusal to surrender to comfort. 
                It is the ability to show up when you are tired, to focus when you are distracted, and to prioritize long-term vision over short-term gratification. You are not defined by your intentions, which are abstract and weightless, but by the consistency of your daily actions. 
                To achieve anything that matters, you must learn to govern your impulses. 
                Discipline is not the absence of desire; it is the presence of intent.</p>
        </div>
        <div class="sc_pic_3">
            <img src="{{ url_for('static', filename='picture/content3.jpg')}}" alt="content1">
            <h4>Doomsday Theories: Are We Facing an Impending End?</h4>
            <p>There is a growing, uneasy murmur in the air—the pervasive sense that we are approaching an endgame for our current way of life. Whether these are mere collective anxieties amplified by modern volatility, 
                or genuine signals of systemic instability, the conversation is shifting. We have built a world of hyper-connectivity, yet this very complexity makes us incredibly brittle. Our reliance on global supply chains, energy grids, and digital 
                infrastructure has created a single point of failure that we rarely acknowledge. If we are indeed staring at the edge of a precipice, then this is our final warning to re-evaluate what is truly essential. It is time to peel back the layers 
                of digital excess and focus on the bedrock of human survival and societal resilience. Panic is a luxury we cannot afford; introspection and preparation are our only logical responses.</p>
        </div>
    </div>

    <h1 class="mainly">My Hacker News</h1>

    <div class ="other">
        <ul class="other_new">
            <li style=" font-weight: bold; margin-left: 20px;">Hacker News</li>
            <li>New</li>
            <li>Past</li>
            <li>Comments</li>
            <li>Ask</li>
            <li>Show</li>
            <li>Submit</li>
        </ul>
        <ol class="other_new2">
            {% for item in new_list %}
                <li><a href="{{ item['Url'] }}">{{ item['Title'] }}</a></li>
            {% endfor %}
        </ol>
    </div>

    <footer>
        <div class="container">
            <div class="footer1">
                <p class="footer_font">Contact</p>
                <p>1093 Lower Delta Road #04-16 <br>Tiong Bahru 2 Singapore 169204</p>
                <p>junhaosia2468@gmail.com</p>
                <p>+65 96174840</p>
            </div>

            <div class="footer2">
                <p class="footer_font">SiteMap</p>
                <p>Home</p>
                <p>News</p>
                <p>About Us</p>
                <p>Contact Us</p>
            </div>

            <div class="footer3">
                <p class="footer_font">Services</p>
                <p>Web Solution</p>
                <p>Upload Your News</p>
                <p>Check The News</p>
            </div>

            <div class="footer4">
                <p class="footer_font">Other Links</p>
                <p>Privacy Policy</p>
                <p>SLA</p>
                <p>Locate Us</p>
                <p>Trust Centre</p>
            </div>

            <div class="footer4">
                <p class="footer_font">Sign Up Here</p>
                <p> Join the stream. Because in a world of constant noise, <br>the ability to filter signal from chaos is the ultimate advantage.</p>
                <div class="sign_up">
                    Please Enter Your Email Here:
                </div>
                <button>SENDEN</button>
            </div>
        </div>
    </footer>
</body>
</html>
