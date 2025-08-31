<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pranav Joshipura - Chief Technology Officer | Chief Digital Officer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #2c3e50;
            background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 20px 60px rgba(0,0,0,0.1);
        }

        .header {
            background: linear-gradient(135deg, #1a365d 0%, #2c5aa0 100%);
            color: white;
            padding: 60px 50px;
            position: relative;
            overflow: hidden;
        }

        .header::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 300px;
            height: 300px;
            background: rgba(255,255,255,0.05);
            border-radius: 50%;
            transform: translate(100px, -100px);
        }

        .header-content {
            position: relative;
            z-index: 2;
        }

        .name {
            font-size: 3.5rem;
            font-weight: 300;
            letter-spacing: -2px;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .title {
            font-size: 1.5rem;
            font-weight: 400;
            opacity: 0.9;
            margin-bottom: 30px;
            font-style: italic;
        }

        .summary {
            font-size: 1.1rem;
            line-height: 1.8;
            max-width: 900px;
            opacity: 0.95;
        }

        .main-content {
            padding: 50px;
        }

        .section {
            margin-bottom: 50px;
            position: relative;
        }

        .section-title {
            font-size: 2.2rem;
            color: #1a365d;
            border-bottom: 3px solid #2c5aa0;
            padding-bottom: 15px;
            margin-bottom: 40px;
            position: relative;
            font-weight: 300;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -3px;
            left: 0;
            width: 60px;
            height: 3px;
            background: #ffd700;
        }

        .experience-item {
            background: #f8f9fa;
            border-left: 4px solid #2c5aa0;
            padding: 30px;
            margin-bottom: 30px;
            border-radius: 0 10px 10px 0;
            transition: all 0.3s ease;
            position: relative;
        }

        .experience-item:hover {
            transform: translateX(10px);
            box-shadow: 0 10px 30px rgba(44, 90, 160, 0.15);
        }

        .job-title {
            font-size: 1.4rem;
            font-weight: 600;
            color: #1a365d;
            margin-bottom: 5px;
        }

        .company {
            font-size: 1.2rem;
            color: #2c5aa0;
            font-weight: 500;
            margin-bottom: 8px;
        }

        .duration-location {
            color: #6c757d;
            font-size: 1rem;
            margin-bottom: 15px;
            font-style: italic;
        }

        .company-description {
            background: rgba(44, 90, 160, 0.05);
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 20px;
            border-left: 3px solid #2c5aa0;
            font-style: italic;
        }

        .achievements {
            list-style: none;
        }

        .achievements li {
            padding: 8px 0;
            border-bottom: 1px solid #dee2e6;
            position: relative;
            padding-left: 25px;
        }

        .achievements li:before {
            content: '▸';
            color: #2c5aa0;
            font-weight: bold;
            position: absolute;
            left: 0;
            font-size: 1.2rem;
        }

        .achievements li:last-child {
            border-bottom: none;
        }

        .education-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
        }

        .education-item {
            background: linear-gradient(135deg, #f8f9fa 0%, #ffffff 100%);
            padding: 25px;
            border-radius: 10px;
            border: 1px solid #dee2e6;
            transition: all 0.3s ease;
        }

        .education-item:hover {
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
            transform: translateY(-5px);
        }

        .degree {
            font-size: 1.2rem;
            font-weight: 600;
            color: #1a365d;
            margin-bottom: 5px;
        }

        .school {
            color: #2c5aa0;
            font-weight: 500;
            margin-bottom: 5px;
        }

        .cert-category {
            background: linear-gradient(135deg, #2c5aa0 0%, #1a365d 100%);
            color: white;
            padding: 15px 25px;
            margin: 20px 0 15px 0;
            border-radius: 8px;
            font-weight: 600;
            font-size: 1.1rem;
        }

        .cert-item {
            background: #f8f9fa;
            padding: 15px 20px;
            margin: 10px 0;
            border-left: 4px solid #ffd700;
            border-radius: 0 8px 8px 0;
        }

        .cert-name {
            font-weight: 600;
            color: #1a365d;
            margin-bottom: 3px;
        }

        .cert-issuer {
            color: #6c757d;
            font-size: 0.9rem;
        }

        .awards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .award-item {
            background: linear-gradient(135deg, #fff3cd 0%, #ffffff 100%);
            padding: 20px;
            border-radius: 10px;
            border: 2px solid #ffd700;
            text-align: center;
            transition: all 0.3s ease;
        }

        .award-item:hover {
            transform: scale(1.02);
            box-shadow: 0 8px 25px rgba(255, 215, 0, 0.3);
        }

        .award-title {
            font-weight: 600;
            color: #1a365d;
            margin-bottom: 5px;
        }

        .award-org {
            color: #6c757d;
            font-size: 0.9rem;
        }

        .highlight-number {
            color: #2c5aa0;
            font-weight: bold;
        }

        @media (max-width: 768px) {
            .main-content {
                padding: 30px 25px;
            }
            
            .header {
                padding: 40px 25px;
            }
            
            .name {
                font-size: 2.5rem;
            }
            
            .education-grid {
                grid-template-columns: 1fr;
            }
            
            .experience-item:hover {
                transform: none;
            }
        }

        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 0.8s ease forwards;
        }

        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .section:nth-child(1) .fade-in { animation-delay: 0.1s; }
        .section:nth-child(2) .fade-in { animation-delay: 0.2s; }
        .section:nth-child(3) .fade-in { animation-delay: 0.3s; }
        .section:nth-child(4) .fade-in { animation-delay: 0.4s; }
    </style>
</head>
<body>
    <div class="container">
        <header class="header">
            <div class="header-content">
                <h1 class="name">Pranav Joshipura</h1>
                <h2 class="title">Chief Technology Officer | Chief Digital Officer</h2>
                <p class="summary">
                    Accomplished digital transformation leader with over <span class="highlight-number">25 years</span> of executive experience leveraging cloud, AI, and modern software practices to evolve legacy systems into scalable platforms that deliver measurable business outcomes. Extensive experience with large-scale engineering leadership, global team management, P&L responsibility, and strategic technology vision.
                </p>
            </div>
        </header>

        <main class="main-content">
            <section class="section">
                <h2 class="section-title fade-in">Professional Experience</h2>
                
                <div class="experience-item fade-in">
                    <h3 class="job-title">Head of Software and Data Engineering, Digital Products and Services</h3>
                    <h4 class="company">Mayo Clinic</h4>
                    <p class="duration-location">October 2021 to Present | Rochester, MN</p>
                    <div class="company-description">
                        Mayo Clinic is a $16B+ global healthcare leader with 70+ locations worldwide, serving millions of patients annually. Report to the Chief Digital Officer and manage 20+ direct reports with a total team size of 400+ engineers across multiple time zones.
                    </div>
                    <ul class="achievements">
                        <li>Led enterprise-wide digital transformation serving <strong>1B+ annual users</strong>, managing <strong>$50M+ technology budget</strong> while partnering with C-suite on strategic technology vision that improved system reliability 30%, performance 70%, and uptime 15%</li>
                        <li>Spearheaded deployment of <strong>generative AI platforms</strong> including enterprise search, clinical AI inference engines for early disease detection, and AI-powered personalization using Adobe Experience Platform, establishing Mayo Clinic as AI-first healthcare leader</li>
                        <li>Orchestrated global Agile/DevOps transformation improving delivery cycles 25% and established offshore development center with 100+ engineers achieving 40% faster hiring and 50% cost savings</li>
                        <li>Built high-velocity software delivery culture leveraging GitHub Copilot and Azure Copilot, increasing development efficiency 20% across API-first, cloud-first, mobile-first architecture</li>
                        <li>Delivered product-oriented delivery model with centralized release management, 90% test automation in Patient Portal, and modern monitoring systems ensuring HIPAA/HITRUST compliance</li>
                    </ul>
                </div>

                <div class="experience-item fade-in">
                    <h3 class="job-title">Director of Engineering & Head of Engineering (Guest Program)</h3>
                    <h4 class="company">Royal Caribbean Group</h4>
                    <p class="duration-location">June 2019 to September 2021 | Miami, FL</p>
                    <div class="company-description">
                        Royal Caribbean Group is a $12B+ global cruise corporation operating 60+ ships across Royal Caribbean, Celebrity, and Azamara brands, serving millions of guests annually. Managed 20+ direct reports with a total team size of 225+ software and automation engineers.
                    </div>
                    <ul class="achievements">
                        <li>Led digital transformation delivering world-class mobile applications (<strong>200M+ users, 4.5+ rating</strong>) using microservices architecture on AWS and on-premise ship/shore infrastructure, generating multi-million dollar revenue impact</li>
                        <li>Spearheaded critical <strong>COVID-19 pandemic response</strong> including contactless guest check-in, revolutionary Muster 2.0 safety system, QR-based digital menus across 40+ ships, and wearable-based contact tracing deployed globally</li>
                        <li>Established "shift-left" DevOps culture with CI/CD automation delivering <strong>multi-million dollar cost savings</strong> through comprehensive platform including telemetry, analytics, accessibility, and monitoring systems</li>
                        <li>Enhanced Adobe Experience Manager-based content management system and integrated diverse global payment methods (AliPay, WeChat Pay) to support international digital commerce initiatives</li>
                        <li>Achieved <strong>4.5+ employee engagement scores</strong> while building next-generation engineering leaders through coaching and Engineering University programs</li>
                    </ul>
                </div>

                <div class="experience-item fade-in">
                    <h3 class="job-title">Senior Director, Head of Product Engineering (Enrollment & Eligibility)</h3>
                    <h4 class="company">Change Healthcare/Optum Insight</h4>
                    <p class="duration-location">April 2014 to May 2019 | Eden Prairie, MN</p>
                    <div class="company-description">
                        Change Healthcare is a healthcare technology company serving 300+ hospitals and health systems with revenue cycle management, clinical decision support, and payment accuracy solutions. Managed $15M budget and led 15+ direct reports with 100+ total team members.
                    </div>
                    <ul class="achievements">
                        <li>Delivered HIPAA-compliant digital transformation of paper-based enrollment processes for <strong>300+ hospitals</strong>, enabling seamless patient enrollment in funding programs and improving payment accessibility</li>
                        <li>Architected Intelligent Data Platform with API-driven architecture for eligibility and enrollment systems, establishing scalable healthcare data infrastructure</li>
                        <li>Led development of Accident Policy Management system from ground zero, enabling new business line growth from <strong>$0 to $10M revenue within one year</strong></li>
                        <li>Pioneered organization's first mobile and cloud application deployed across 300+ hospitals using AWS microservices architecture</li>
                        <li>Built test-driven development culture and automated 2K+ scripts, achieved multiple AWS certifications across team members</li>
                    </ul>
                </div>

                <div class="experience-item fade-in">
                    <h3 class="job-title">Previous Leadership Roles</h3>
                    <ul class="achievements">
                        <li><strong>Technical Manager</strong> | Computer Science Corporation (May 2007 - September 2012)</li>
                        <li><strong>Director, App Development & Support</strong> | Heath Care Excel (February 2005 - February 2007)</li>
                        <li><strong>Software Engineer/Analyst Programmer</strong> | Friedrich Klatt & Associates (September 2002 - February 2005)</li>
                    </ul>
                </div>
            </section>

            <section class="section">
                <h2 class="section-title fade-in">Education</h2>
                <div class="education-grid fade-in">
                    <div class="education-item">
                        <div class="degree">Master of Science, Computer Science</div>
                        <div class="school">Illinois Institute of Technology</div>
                        <div class="duration-location">May 2003 | Chicago, IL</div>
                    </div>
                    <div class="education-item">
                        <div class="degree">Bachelor of Engineering</div>
                        <div class="school">L D College of Engineering</div>
                        <div class="duration-location">May 2000 | India | <em>Distinction</em></div>
                    </div>
                </div>
            </section>

            <section class="section">
                <h2 class="section-title fade-in">Professional Certifications</h2>
                
                <div class="fade-in">
                    <div class="cert-category">AI & Machine Learning Leadership</div>
                    <div class="cert-item">
                        <div class="cert-name">Google Cloud Certified Generative AI Leader</div>
                        <div class="cert-issuer">Google Cloud</div>
                    </div>
                    <div class="cert-item">
                        <div class="cert-name">GitHub Copilot Certified</div>
                        <div class="cert-issuer">Microsoft</div>
                    </div>

                    <div class="cert-category">Cloud & DevOps Architecture</div>
                    <div class="cert-item">
                        <div class="cert-name">Google Cloud Certified Professional Cloud Architect</div>
                        <div class="cert-issuer">Google Cloud</div>
                    </div>
                    <div class="cert-item">
                        <div class="cert-name">AWS Certified Solutions Architect - Professional</div>
                        <div class="cert-issuer">Amazon Web Services</div>
                    </div>
                    <div class="cert-item">
                        <div class="cert-name">Google Cloud Certified Professional Cloud DevOps Engineer</div>
                        <div class="cert-issuer">Google Cloud</div>
                    </div>

                    <div class="cert-category">Agile Transformation</div>
                    <div class="cert-item">
                        <div class="cert-name">Certified SAFe 5 Agilist</div>
                        <div class="cert-issuer">Scaled Agile Framework</div>
                    </div>

                    <div class="cert-category">Executive Leadership Development</div>
                    <div class="cert-item">
                        <div class="cert-name">DRIVE - Executive Leadership Program (10 Months)</div>
                        <div class="cert-issuer">Mayo Clinic</div>
                    </div>
                    <div class="cert-item">
                        <div class="cert-name">Mastering the Art of Management (8 Months)</div>
                        <div class="cert-issuer">Situational Leadership, Performance Management, Building High Performing Teams</div>
                    </div>
                </div>
            </section>

            <section class="section">
                <h2 class="section-title fade-in">Recognition & Awards</h2>
                <div class="awards-grid fade-in">
                    <div class="award-item">
                        <div class="award-title">Leadership Recognition Champion - RICH TIES Values</div>
                        <div class="award-org">Mayo Clinic</div>
                    </div>
                    <div class="award-item">
                        <div class="award-title">Exceptional Leadership in Royal Caribbean Digital Transformation</div>
                        <div class="award-org">Royal Caribbean Group</div>
                    </div>
                    <div class="award-item">
                        <div class="award-title">Exceptional Leadership in Georgia Medicaid Portal Development</div>
                        <div class="award-org">State of Georgia Leadership</div>
                    </div>
                    <div class="award-item">
                        <div class="award-title">Pinnacle Award and Cloud Transformation Award</di
