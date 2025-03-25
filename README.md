<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elite IPTV - A Experiência Definitiva em Streaming</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@700;800;900&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #0f172a;
            --secondary: #3b82f6;
            --accent: #f59e0b;
            --dark: #1e293b;
            --light: #f8fafc;
            --success: #10b981;
            --danger: #ef4444;
            --portugal: #046a38;
            --brasil: #fcd116;
            --transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--primary);
            color: var(--light);
            overflow-x: hidden;
            line-height: 1.7;
        }
        
        h1, h2, h3, h4 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 800;
        }
        
        /* Header Hero Section */
        .hero {
            min-height: 100vh;
            background: linear-gradient(135deg, rgba(15, 23, 42, 0.9), rgba(15, 23, 42, 0.95)), 
                        url('https://images.unsplash.com/photo-1605106702734-205df224ecce?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80') no-repeat center center/cover;
            position: relative;
            overflow: hidden;
            display: flex;
            align-items: center;
            padding: 0 2rem;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 100%;
            height: 100px;
            background: url('data:image/svg+xml;utf8,<svg viewBox="0 0 1200 120" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none"><path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" fill="%23f8fafc" opacity=".25"/><path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" fill="%23f8fafc" opacity=".5"/><path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" fill="%23f8fafc"/></svg>');
            background-size: cover;
            z-index: 10;
        }
        
        .hero-content {
            max-width: 1200px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
            text-align: center;
            padding: 4rem 0;
        }
        
        .hero h1 {
            font-size: 4.5rem;
            margin-bottom: 1.5rem;
            background: linear-gradient(to right, var(--light), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            line-height: 1.2;
            animation: fadeInUp 1s ease;
        }
        
        .hero p {
            font-size: 1.25rem;
            max-width: 700px;
            margin: 0 auto 2.5rem;
            color: rgba(248, 250, 252, 0.8);
            animation: fadeInUp 1s ease 0.2s forwards;
            opacity: 0;
        }
        
        .cta-button {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, var(--secondary), var(--accent));
            color: white;
            padding: 1rem 2.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: var(--transition);
            box-shadow: 0 10px 20px rgba(59, 130, 246, 0.3);
            animation: fadeInUp 1s ease 0.4s forwards;
            opacity: 0;
            position: relative;
            overflow: hidden;
            z-index: 1;
        }
        
        .cta-button:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(59, 130, 246, 0.4);
        }
        
        .cta-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, var(--accent), var(--secondary));
            z-index: -1;
            opacity: 0;
            transition: var(--transition);
        }
        
        .cta-button:hover::before {
            opacity: 1;
        }
        
        .cta-button i {
            margin-left: 10px;
            transition: var(--transition);
        }
        
        .cta-button:hover i {
            transform: translateX(5px);
        }
        
        .floating-devices {
            position: relative;
            height: 400px;
            margin-top: 5rem;
            animation: float 6s ease-in-out infinite;
        }
        
        .device {
            position: absolute;
            border-radius: 15px;
            box-shadow: 0 30px 50px rgba(0, 0, 0, 0.3);
            overflow: hidden;
            transition: var(--transition);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .device img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .tv {
            width: 500px;
            height: 300px;
            left: 50%;
            transform: translateX(-50%);
            z-index: 3;
            animation: float 6s ease-in-out infinite 0.5s;
        }
        
        .tablet {
            width: 250px;
            height: 350px;
            left: 20%;
            bottom: 0;
            z-index: 2;
            animation: float 6s ease-in-out infinite 0.2s;
        }
        
        .phone {
            width: 150px;
            height: 250px;
            right: 20%;
            bottom: 0;
            z-index: 1;
            animation: float 6s ease-in-out infinite 0.7s;
        }
        
        /* Features Section */
        .features {
            padding: 8rem 2rem;
            background-color: var(--light);
            position: relative;
        }
        
        .features::before {
            content: '';
            position: absolute;
            top: -10px;
            left: 0;
            width: 100%;
            height: 100px;
            background: url('data:image/svg+xml;utf8,<svg viewBox="0 0 1200 120" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none"><path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" fill="%230f172a" opacity=".25"/><path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" fill="%230f172a" opacity=".5"/><path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" fill="%230f172a"/></svg>');
            background-size: cover;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 5rem;
            color: var(--primary);
        }
        
        .section-title h2 {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            position: relative;
            display: inline-block;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(to right, var(--secondary), var(--accent));
            border-radius: 2px;
        }
        
        .section-title p {
            font-size: 1.2rem;
            color: var(--dark);
            max-width: 700px;
            margin: 0 auto;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .feature-card {
            background: white;
            border-radius: 15px;
            padding: 2.5rem;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
            z-index: 1;
            color: var(--dark);
        }
        
        .feature-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 4px;
            height: 0;
            background: linear-gradient(to bottom, var(--secondary), var(--accent));
            transition: var(--transition);
            z-index: -1;
        }
        
        .feature-card:hover::before {
            height: 100%;
            width: 100%;
            opacity: 0.1;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
            color: var(--secondary);
        }
        
        .feature-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }
        
        .feature-card p {
            color: var(--dark);
            opacity: 0.8;
            margin-bottom: 1.5rem;
        }
        
        .channel-list {
            columns: 2;
            margin-top: 1rem;
        }
        
        .channel-list li {
            margin-bottom: 0.75rem;
            list-style-type: none;
            position: relative;
            padding-left: 1.75rem;
            color: var(--dark);
            opacity: 0.9;
        }
        
        .channel-list li:before {
            content: "✓";
            color: var(--success);
            position: absolute;
            left: 0;
            font-weight: bold;
        }
        
        /* Pricing Section */
        .pricing {
            padding: 8rem 2rem;
            background-color: var(--primary);
            position: relative;
        }
        
        .pricing::before {
            content: '';
            position: absolute;
            top: -10px;
            left: 0;
            width: 100%;
            height: 100px;
            background: url('data:image/svg+xml;utf8,<svg viewBox="0 0 1200 120" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none"><path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" fill="%23f8fafc" opacity=".25"/><path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" fill="%23f8fafc" opacity=".5"/><path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" fill="%23f8fafc"/></svg>');
            background-size: cover;
        }
        
        .country-tabs {
            display: flex;
            justify-content: center;
            margin-bottom: 3rem;
            background: rgba(248, 250, 252, 0.1);
            padding: 10px;
            border-radius: 50px;
            max-width: 500px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .tab-button {
            padding: 12px 30px;
            background: transparent;
            border: none;
            cursor: pointer;
            font-size: 1rem;
            font-weight: 600;
            color: var(--light);
            opacity: 0.7;
            transition: var(--transition);
            border-radius: 30px;
            display: flex;
            align-items: center;
        }
        
        .tab-button i {
            margin-right: 8px;
        }
        
        .tab-button.active {
            opacity: 1;
            background: rgba(59, 130, 246, 0.2);
            color: white;
        }
        
        .tab-button.brasil.active {
            background: rgba(252, 209, 22, 0.2);
        }
        
        .tab-button.portugal.active {
            background: rgba(4, 106, 56, 0.2);
        }
        
        .pricing-cards {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .pricing-card {
            background: rgba(30, 41, 59, 0.7);
            border-radius: 15px;
            padding: 3rem 2rem;
            width: 350px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
        }
        
        .pricing-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.3);
            border-color: rgba(59, 130, 246, 0.3);
        }
        
        .popular {
            border: 1px solid var(--accent);
        }
        
        .popular .plan-name::after {
            content: 'MAIS POPULAR';
            position: absolute;
            top: 15px;
            right: -30px;
            background: var(--accent);
            color: var(--primary);
            padding: 3px 30px;
            font-size: 0.7rem;
            font-weight: 800;
            transform: rotate(45deg);
            width: 150px;
            text-align: center;
        }
        
        .plan-name {
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
            color: var(--light);
            position: relative;
            text-align: center;
        }
        
        .plan-price {
            font-size: 3.5rem;
            font-weight: 800;
            color: white;
            margin-bottom: 0.5rem;
            text-align: center;
            line-height: 1;
        }
        
        .plan-price span {
            font-size: 1rem;
            font-weight: normal;
            opacity: 0.7;
        }
        
        .plan-period {
            text-align: center;
            display: block;
            margin-bottom: 2rem;
            color: rgba(255, 255, 255, 0.7);
        }
        
        .plan-features {
            margin: 2.5rem 0;
        }
        
        .plan-features li {
            margin-bottom: 1rem;
            list-style-type: none;
            position: relative;
            padding-left: 2rem;
            color: rgba(255, 255, 255, 0.9);
        }
        
        .plan-features li:before {
            content: "✓";
            color: var(--success);
            position: absolute;
            left: 0;
            font-weight: bold;
        }
        
        .plan-button {
            display: block;
            text-align: center;
            background: linear-gradient(135deg, var(--secondary), var(--accent));
            color: white;
            padding: 1rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: var(--transition);
            margin-top: 2rem;
        }
        
        .plan-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(59, 130, 246, 0.3);
        }
        
        /* Testimonials Section */
        .testimonials {
            padding: 8rem 2rem;
            background-color: var(--light);
            position: relative;
        }
        
        .testimonials::before {
            content: '';
            position: absolute;
            top: -10px;
            left: 0;
            width: 100%;
            height: 100px;
            background: url('data:image/svg+xml;utf8,<svg viewBox="0 0 1200 120" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none"><path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" fill="%230f172a" opacity=".25"/><path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" fill="%230f172a" opacity=".5"/><path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" fill="%230f172a"/></svg>');
            background-size: cover;
        }
        
        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .testimonial-card {
            background: white;
            border-radius: 15px;
            padding: 2.5rem;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            transition: var(--transition);
            position: relative;
        }
        
        .testimonial-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
        }
        
        .testimonial-card::before {
            content: '"';
            position: absolute;
            top: 20px;
            left: 20px;
            font-size: 5rem;
            font-family: Georgia, serif;
            color: rgba(59, 130, 246, 0.1);
            line-height: 1;
            z-index: 0;
        }
        
        .testimonial-text {
            position: relative;
            z-index: 1;
            font-style: italic;
            margin-bottom: 1.5rem;
            color: var(--dark);
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .author-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            overflow: hidden;
            margin-right: 1rem;
            background: var(--primary);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
            font-size: 1.2rem;
        }
        
        .author-info h4 {
            color: var(--primary);
            margin-bottom: 0.2rem;
        }
        
        .author-info p {
            color: var(--dark);
            opacity: 0.7;
            font-size: 0.9rem;
        }
        
        /* FAQ Section */
        .faq {
            padding: 8rem 2rem;
            background-color: var(--primary);
            position: relative;
        }
        
        .faq::before {
            content: '';
            position: absolute;
            top: -10px;
            left: 0;
            width: 100%;
            height: 100px;
            background: url('data:image/svg+xml;utf8,<svg viewBox="0 0 1200 120" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none"><path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" fill="%23f8fafc" opacity=".25"/><path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" fill="%23f8fafc" opacity=".5"/><path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" fill="%23f8fafc"/></svg>');
            background-size: cover;
        }
        
        .faq-container {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .faq-item {
            margin-bottom: 1rem;
            border-radius: 10px;
            overflow: hidden;
            background: rgba(30, 41, 59, 0.7);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .faq-question {
            padding: 1.5rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            cursor: pointer;
            font-weight: 600;
            transition: var(--transition);
        }
        
        .faq-question:hover {
            background: rgba(59, 130, 246, 0.1);
        }
        
        .faq-question i {
            transition: var(--transition);
        }
        
        .faq-answer {
            padding: 0 1.5rem;
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease, padding 0.3s ease;
            color: rgba(255, 255, 255, 0.8);
        }
        
        .faq-item.active .faq-question {
            background: rgba(59, 130, 246, 0.2);
        }
        
        .faq-item.active .faq-question i {
            transform: rotate(180deg);
        }
        
        .faq-item.active .faq-answer {
            max-height: 500px;
            padding: 0 1.5rem 1.5rem;
        }
        
        /* CTA Section */
        .final-cta {
            padding: 8rem 2rem;
            background: linear-gradient(135deg, rgba(15, 23, 42, 0.9), rgba(15, 23, 42, 0.95)), 
                        url('https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80') no-repeat center center/cover;
            text-align: center;
            position: relative;
        }
        
        .final-cta h2 {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            color: white;
        }
        
        .final-cta p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 3rem;
            color: rgba(255, 255, 255, 0.8);
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            padding: 5rem 2rem 2rem;
            position: relative;
        }
        
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 3rem;
        }
        
        .footer-logo {
            font-size: 1.8rem;
            font-weight: 800;
            margin-bottom: 1.5rem;
            color: white;
        }
        
        .footer-about p {
            color: rgba(255, 255, 255, 0.7);
            margin-bottom: 1.5rem;
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
        }
        
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            transition: var(--transition);
        }
        
        .social-links a:hover {
            background: var(--secondary);
            transform: translateY(-3px);
        }
        
        .footer-links h3 {
            color: white;
            font-size: 1.2rem;
            margin-bottom: 1.5rem;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-links h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 40px;
            height: 3px;
            background: var(--secondary);
        }
        
        .footer-links ul li {
            margin-bottom: 0.8rem;
            list-style: none;
        }
        
        .footer-links ul li a {
            color: rgba(255, 255, 255, 0.7);
            text-decoration: none;
            transition: var(--transition);
        }
        
        .footer-links ul li a:hover {
            color: var(--secondary);
            padding-left: 5px;
        }
        
        .footer-contact p {
            display: flex;
            align-items: center;
            color: rgba(255, 255, 255, 0.7);
            margin-bottom: 1rem;
        }
        
        .footer-contact i {
            margin-right: 10px;
            color: var(--secondary);
        }
        
        .copyright {
            text-align: center;
            margin-top: 4rem;
            padding-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: rgba(255, 255, 255, 0.5);
            font-size: 0.9rem;
        }
        
        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes float {
            0% {
                transform: translateY(0px);
            }
            50% {
                transform: translateY(-20px);
            }
            100% {
                transform: translateY(0px);
            }
        }
        
        /* Responsive Styles */
        @media (max-width: 992px) {
            .hero h1 {
                font-size: 3.5rem;
            }
            
            .pricing-cards {
                flex-direction: column;
                align-items: center;
            }
            
            .pricing-card {
                width: 100%;
                max-width: 400px;
            }
        }
        
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero p {
                font-size: 1.1rem;
            }
            
            .section-title h2 {
                font-size: 2.2rem;
            }
            
            .final-cta h2 {
                font-size: 2.2rem;
            }
            
            .floating-devices {
                height: 300px;
                margin-top: 3rem;
            }
            
            .tv {
                width: 350px;
                height: 210px;
            }
            
            .tablet {
                width: 175px;
                height: 245px;
                left: 10%;
            }
            
            .phone {
                width: 105px;
                height: 175px;
                right: 10%;
            }
        }
        
        @media (max-width: 576px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .country-tabs {
                flex-direction: column;
                border-radius: 15px;
                padding: 15px;
                gap: 10px;
            }
            
            .tab-button {
                border-radius: 10px !important;
                justify-content: center;
            }
            
            .channel-list {
                columns: 1;
            }
        }
    </style>
</head>
<body>
    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>A Melhor Experiência em IPTV Premium</h1>
            <p>Mais de 10.000 conteúdos em alta definição, sem travamentos e com a melhor seleção de canais para Brasil e Portugal. Assista em qualquer dispositivo, a qualquer hora.</p>
            <a href="#pricing" class="cta-button">ASSINE AGORA <i class="fas fa-arrow-right"></i></a>
            
            <div class="floating-devices">
                <div class="device tv">
                    <img src="https://images.unsplash.com/photo-1574375927938-d5a98e8ffe85?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1496&q=80" alt="IPTV na TV">
                </div>
                <div class="device tablet">
                    <img src="https://images.unsplash.com/photo-1593784991095-a205069470b6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="IPTV no Tablet">
                </div>
                <div class="device phone">
                    <img src="https://images.unsplash.com/photo-1601784551446-20c9e07cdbdb?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1467&q=80" alt="IPTV no Celular">
                </div>
            </div>
        </div>
    </section>
    
    <!-- Features Section -->
    <section class="features">
        <div class="section-title">
            <h2>O Que Oferecemos</h2>
            <p>Descubra por que somos a escolha premium para milhares de clientes satisfeitos em Brasil e Portugal</p>
        </div>
        
        <div class="features-grid">
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-film"></i></div>
                <h3>Filmes Premium</h3>
                <p>+230 lançamentos recentes em qualidade Full HD</p>
                <ul class="channel-list">
                    <li>Filmes infantis (últimos lançamentos)</li>
                    <li>Ação, comédia, drama, terror</li>
                    <li>Clássicos do cinema</li>
                    <li>Atualizações semanais</li>
                    <li>Dublados e legendados</li>
                    <li>Qualidade 4K disponível</li>
                </ul>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-tv"></i></div>
                <h3>Séries Completas</h3>
                <p>Todas as plataformas em um só lugar</p>
                <ul class="channel-list">
                    <li>Netflix, Prime Video, HBO Max</li>
                    <li>Disney+, Apple TV+, Star+</li>
                    <li>Séries nacionais e internacionais</li>
                    <li>Episódios atualizados diariamente</li>
                    <li>Temporadas completas</li>
                    <li>Conteúdo exclusivo</li>
                </ul>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-futbol"></i></div>
                <h3>Esportes ao Vivo</h3>
                <p>Transmissões em tempo real em HD</p>
                <ul class="channel-list">
                    <li>+300 canais esportivos BR</li>
                    <li>80+ canais esportivos PT</li>
                    <li>Futebol nacional e internacional</li>
                    <li>Fórmula 1, NBA, NFL, UFC</li>
                    <li>Canais premium: ESPN, Fox Sports</li>
                    <li>Eventos PPV inclusos</li>
                </ul>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-globe-americas"></i></div>
                <h3>Canais Internacionais</h3>
                <p>Diversidade cultural em vários idiomas</p>
                <ul class="channel-list">
                    <li>300+ canais brasileiros</li>
                    <li>80+ canais portugueses</li>
                    <li>Canais infantis dedicados</li>
                    <li>Noticiários 24/7</li>
                    <li>Documentários e cultura</li>
                    <li>Em breve mais países</li>
                </ul>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-child"></i></div>
                <h3>Conteúdo Infantil</h3>
                <p>Seguro e educativo para todas as idades</p>
                <ul class="channel-list">
                    <li>Desenhos animados</li>
                    <li>Filmes educativos</li>
                    <li>Programas infantis</li>
                    <li>Conteúdo sem violência</li>
                    <li>Dublagem profissional</li>
                    <li>Atualizações diárias</li>
                </ul>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon"><i class="fas fa-medal"></i></div>
                <h3>Vantagens Exclusivas</h3>
                <p>Por que somos a melhor escolha</p>
                <ul class="channel-list">
                    <li>Sinal 99.9% estável</li>
                    <li>Qualidade Full HD/4K</li>
                    <li>Suporte 24/7 dedicado</li>
                    <li>Preços competitivos</li>
                    <li>Multiplataforma</li>
                    <li>Atualizações constantes</li>
                </ul>
            </div>
        </div>
    </section>
    
    <!-- Pricing Section -->
    <section class="pricing" id="pricing">
        <div class="section-title">
            <h2>Nossos Planos</h2>
            <p>Escolha o pacote perfeito para suas necessidades. Todos os planos incluem teste gratuito de 24 horas.</p>
        </div>
        
        <div class="country-tabs">
            <button class="tab-button brasil active" onclick="showPricing('brasil')">
                <i class="fas fa-flag"></i> Pacotes Brasil
            </button>
            <button class="tab-button portugal" onclick="showPricing('portugal')">
                <i class="fas fa-flag"></i> Pacotes Portugal
            </button>
        </div>
        
        <!-- Planos para Brasil -->
        <div id="brasil-pricing" class="pricing-content">
            <div class="pricing-cards">
                <div class="pricing-card">
                    <h3 class="plan-name">BÁSICO</h3>
                    <div class="plan-price">R$29<span class="plan-period">/mês</span></div>
                    <div class="plan-features">
                        <ul>
                            <li>+300 canais brasileiros</li>
                            <li>100+ filmes mensais</li>
                            <li>50+ séries atualizadas</li>
                            <li>1 dispositivo simultâneo</li>
                            <li>Suporte por e-mail</li>
                            <li>Qualidade Full HD</li>
                        </ul>
                    </div>
                    <a href="#" class="plan-button">ASSINAR AGORA</a>
                </div>
                
                <div class="pricing-card popular">
                    <h3 class="plan-name">PREMIUM</h3>
                    <div class="plan-price">R$69<span class="plan-period">/3 meses</span></div>
                    <div class="plan-features">
                        <ul>
                            <li>Todos os canais brasileiros</li>
                            <li>+230 filmes mensais</li>
                            <li>Todas as séries completas</li>
                            <li>3 dispositivos simultâneos</li>
                            <li>Suporte prioritário 24/7</li>
                            <li>Qualidade até 4K</li>
                        </ul>
                    </div>
                    <a href="#" class="plan-button">ASSINAR AGORA</a>
                </div>
                
                <div class="pricing-card">
                    <h3 class="plan-name">FAMÍLIA</h3>
                    <div class="plan-price">R$229<span class="plan-period">/ano</span></div>
                    <div class="plan-features">
                        <ul>
                            <li>Todos os canais + internacionais</li>
                            <li>Catálogo completo de filmes</li>
                            <li>Todas as séries + conteúdo exclusivo</li>
                            <li>5 dispositivos simultâneos</li>
                            <li>Suporte VIP personalizado</li>
                            <li>Qualidade máxima 4K HDR</li>
                        </ul>
                    </div>
                    <a href="#" class="plan-button">ASSINAR AGORA</a>
                </div>
            </div>
        </div>
        
        <!-- Planos para Portugal -->
        <div id="portugal-pricing" class="pricing-content" style="display: none;">
            <div class="pricing-cards">
                <div class="pricing-card">
                    <h3 class="plan-name">BÁSICO</h3>
                    <div class="plan-price">€9<span class="plan-period">/mês</span></div>
                    <div class="plan-features">
                        <ul>
                            <li>80+ canais portugueses</li>
                            <li>50+ filmes mensais</li>
                            <li>30+ séries atualizadas</li>
                            <li>1 dispositivo simultâneo</li>
                            <li>Suporte por e-mail</li>
                            <li>Qualidade HD</li>
                        </ul>
                    </div>
                    <a href="#" class="plan-button">ASSINAR AGORA</a>
                </div>
                
                <div class="pricing-card popular">
                    <h3 class="plan-name">PREMIUM</h3>
                    <div class="plan-price">€25<span class="plan-period">/3 meses</span></div>
                    <div class="plan-features">
                        <ul>
                            <li>Todos os canais portugueses</li>
                            <li>150+ filmes mensais</li>
                            <li>70+ séries completas</li>
                            <li>3 dispositivos simultâneos</li>
                            <li>Suporte prioritário 24/7</li>
                            <li>Qualidade Full HD</li>
                        </ul>
                    </div>
                    <a href="#" class="plan-button">ASSINAR AGORA</a>
                </div>
                
                <div class="pricing-card">
                    <h3 class="plan-name">FAMÍLIA</h3>
                    <div class="plan-price">€79<span class="plan-period">/ano</span></div>
                    <div class="plan-features">
                        <ul>
                            <li>Todos os canais + internacionais</li>
                            <li>Catálogo completo de filmes</li>
                            <li>Todas as séries + conteúdo exclusivo</li>
                            <li>5 dispositivos simultâneos</li>
                            <li>Suporte VIP personalizado</li>
                            <li>Qualidade máxima 4K</li>
                        </ul>
                    </div>
                    <a href="#" class="plan-button">ASSINAR AGORA</a>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Testimonials Section -->
    <section class="testimonials">
        <div class="section-title">
            <h2>O Que Nossos Clientes Dizem</h2>
            <p>Avaliações reais de usuários satisfeitos com nosso serviço</p>
        </div>
        
        <div class="testimonials-grid">
            <div class="testimonial-card">
                <p class="testimonial-text">"Finalmente encontrei um IPTV que realmente funciona sem travamentos. A qualidade da imagem é incrível e o catálogo de filmes atualizados me surpreendeu. Recomendo para todos que querem economizar sem perder qualidade."</p>
                <div class="testimonial-author">
                    <div class="author-avatar">CS</div>
                    <div class="author-info">
                        <h4>Carlos Silva</h4>
                        <p>São Paulo, Brasil</p>
                    </div>
                </div>
            </div>
            
            <div class="testimonial-card">
                <p class="testimonial-text">"Como portuguesa vivendo no Brasil, este serviço foi a solução perfeita para manter acesso aos canais portugueses que amo. A variedade de conteúdo e a estabilidade da conexão superaram todas as minhas expectativas."</p>
                <div class="testimonial-author">
                    <div class="author-avatar">MF</div>
                    <div class="author-info">
                        <h4>Maria Fernandes</h4>
                        <p>Rio de Janeiro, Brasil</p>
                    </div>
                </div>
            </div>
            
            <div class="testimonial-card">
                <p class="testimonial-text">"O suporte técnico é excepcional - resolveram meu problema em minutos. Os canais esportivos em Full HD são perfeitos para assistir a todos os jogos do meu time. Vale cada centavo pelo plano anual!"</p>
                <div class="testimonial-author">
                    <div class="author-avatar">JS</div>
                    <div class="author-info">
                        <h4>João Santos</h4>
                        <p>Porto, Portugal</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- FAQ Section -->
    <section class="faq">
        <div class="section-title">
            <h2>Perguntas Frequentes</h2>
            <p>Tire suas dúvidas sobre nosso serviço IPTV premium</p>
        </div>
        
        <div class="faq-container">
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFaq(this)">
                    <span>Como posso testar o serviço antes de comprar?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Oferecemos um teste gratuito de 24 horas para que você possa experimentar nossa qualidade e estabilidade. Basta entrar em contato com nosso suporte via WhatsApp ou Telegram para solicitar seu acesso de teste.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFaq(this)">
                    <span>Quais dispositivos são compatíveis?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Nosso serviço é compatível com Smart TVs (Android TV, Samsung, LG), dispositivos móveis (Android/iOS), computadores (Windows/Mac), e aparelhos como Amazon Fire Stick, Chromecast, Android Box e muito mais. Fornecemos aplicativos dedicados e instruções detalhadas para cada plataforma.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFaq(this)">
                    <span>Como é feita a renovação dos planos?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>A renovação é automática apenas para planos mensais. Planos trimestrais e anuais requerem renovação manual, enviaremos lembretes por e-mail e WhatsApp antes do vencimento. Não cobramos automaticamente sem autorização para planos de longo prazo.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFaq(this)">
                    <span>O serviço funciona fora do Brasil/Portugal?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Sim! Nosso serviço foi otimizado para funcionar em qualquer país do mundo. Recomendamos uma conexão de internet estável com pelo menos 10mbps para Full HD e 25mbps para conteúdo 4K.</p>
                </div>
            </div>
            
            <div class="faq-item">
                <div class="faq-question" onclick="toggleFaq(this)">
                    <span>Como é o suporte técnico oferecido?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    <p>Oferecemos suporte 24/7 via WhatsApp, Telegram e e-mail. Nossos tempos médios de resposta são: 5 minutos para clientes Premium/Família e 30 minutos para clientes Básicos. Também temos tutoriais em vídeo e guias passo-a-passo para configuração.</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Final CTA Section -->
    <section class="final-cta">
        <h2>Pronto para Transformar Sua Experiência de TV?</h2>
        <p>Junte-se a milhares de clientes satisfeitos e tenha acesso ao melhor conteúdo em qualidade premium</p>
        <a href="#pricing" class="cta-button">ASSINE AGORA <i class="fas fa-arrow-right"></i></a>
    </section>
    
    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-about">
                <div class="footer-logo">ELITE IPTV</div>
                <p>A experiência definitiva em streaming para Brasil e Portugal. Qualidade premium, conteúdo exclusivo e suporte dedicado.</p>
                <div class="social-links">
                    <a href="#"><i class="fab fa-whatsapp"></i></a>
                    <a href="#"><i class="fab fa-telegram"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-facebook"></i></a>
                </div>
            </div>
            
            <div class="footer-links">
                <h3>Links Rápidos</h3>
                <ul>
                    <li><a href="#">Início</a></li>
                    <li><a href="#pricing">Planos</a></li>
                    <li><a href="#">Canais</a></li>
                    <li><a href="#">Aplicativos</a></li>
                    <li><a href="#">Tutoriais</a></li>
                    <li><a href="#">Blog</a></li>
                </ul>
            </div>
            
            <div class="footer-links">
                <h3>Serviços</h3>
                <ul>
                    <li><a href="#">IPTV para Brasil</a></li>
                    <li><a href="#">IPTV para Portugal</a></li>
                    <li><a href="#">Pacote Esportivo</a></li>
                    <li><a href="#">Pacote Infantil</a></li>
                    <li><a href="#">Pacote Cinema</a></li>
                    <li><a href="#">Configurações</a></li>
                </ul>
            </div>
            
            <div class="footer-contact">
                <h3>Contato</h3>
                <p><i class="fas fa-phone-alt"></i> +55 (11) 98765-4321</p>
                <p><i class="fas fa-phone-alt"></i> +351 912 345 678</p>
                <p><i class="fas fa-envelope"></i> suporte@eliteiptv.com</p>
                <p><i class="fas fa-clock"></i> Suporte 24/7</p>
            </div>
        </div>
        
        <div class="copyright">
            <p>&copy; 2023 Elite IPTV. Todos os direitos reservados. | <a href="#">Termos de Serviço</a> | <a href="#">Política de Privacidade</a></p>
        </div>
    </footer>
    
    <script>
        // Mostrar planos por país
        function showPricing(country) {
            // Esconde todos os conteúdos de preço
            document.querySelectorAll('.pricing-content').forEach(content => {
                content.style.display = 'none';
            });
            
            // Mostra apenas o conteúdo do país selecionado
            document.getElementById(country + '-pricing').style.display = 'block';
            
            // Atualiza os botões de tab
            document.querySelectorAll('.tab-button').forEach(button => {
                button.classList.remove('active');
            });
            
            document.querySelector('.tab-button.' + country).classList.add('active');
        }
        
        // Alternar FAQ
        function toggleFaq(question) {
            const faqItem = question.parentElement;
            faqItem.classList.toggle('active');
        }
        
        // Animação ao rolar a página
        document.addEventListener('DOMContentLoaded', function() {
            const animateOnScroll = function() {
                const elements = document.querySelectorAll('.feature-card, .pricing-card, .testimonial-card');
                
                elements.forEach(element => {
                    const elementPosition = element.getBoundingClientRect().top;
                    const windowHeight = window.innerHeight;
                    
                    if (elementPosition < windowHeight - 100) {
                        element.style.opacity = '1';
                        element.style.transform = 'translateY(0)';
                    }
                });
            };
            
            // Inicializa elementos com opacidade 0 para animação
            const animatedElements = document.querySelectorAll('.feature-card, .pricing-card, .testimonial-card');
            animatedElements.forEach(element => {
                element.style.opacity = '0';
                element.style.transform = 'translateY(30px)';
                element.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            });
            
            window.addEventListener('scroll', animateOnScroll);
            animateOnScroll(); // Executa uma vez ao carregar
        });
    </script>
</body>
</html>
