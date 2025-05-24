<html lang="ko"><head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GKS 학교 급식표</title>
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #2980b9;
            --accent-color: #e74c3c;
            --light-bg: rgba(255, 255, 255, 0.9);
            --dark-text: #333;
            --light-text: #fff;
        }
        
        body {
            font-family: 'Nanum Gothic', 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            color: var(--dark-text);
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            min-height: 100vh;
        }
        
        /* 헤더 스타일 */
        header {
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            color: var(--light-text);
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }
        
        /* 내용을 감싸는 컨테이너 */
        .container {
            max-width: 1000px;
            margin: 30px auto;
            padding: 30px;
            background-color: var(--light-text);
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        h1 {
            color: var(--primary-color);
            text-align: center;
            margin-bottom: 30px;
            font-size: 2.2em;
        }
        
        /* 링크 버튼 컨테이너 */
        .button-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            margin-bottom: 40px;
            gap: 15px;
        }
        
        /* 링크 버튼 스타일 */
        .link-button {
            padding: 15px 30px;
            background-color: var(--primary-color);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: all 0.3s ease;
            text-align: center;
            min-width: 180px;
            box-shadow: 0 4px 8px rgba(52, 152, 219, 0.3);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100px;
        }
        
        .link-button i {
            font-size: 24px;
            margin-bottom: 8px;
        }
        
        .link-button:hover {
            background-color: var(--secondary-color);
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(41, 128, 185, 0.4);
        }
        
        /* 급식표 섹션 */
        .meal-section {
            margin-top: 40px;
            animation: fadeIn 0.8s ease;
        }
        
        /* 날짜 표시 */
        .current-date {
            text-align: center;
            font-size: 1.2em;
            margin-bottom: 20px;
            color: var(--secondary-color);
            font-weight: bold;
        }
        
        /* 급식표 스타일 */
        .meal-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            background-color: white;
            color: var(--dark-text);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            border-radius: 10px;
            overflow: hidden;
        }
        
        .meal-table th, .meal-table td {
            border: 1px solid #e0e0e0;
            padding: 15px;
            text-align: center;
        }
        
        .meal-table th {
            background-color: var(--primary-color);
            color: white;
            font-weight: 600;
        }
        
        .meal-table tr:nth-child(even) {
            background-color: #f8f9fa;
        }
        
        .meal-table tr:hover {
            background-color: #e9f7fe;
        }
        
        /* 날짜 선택기 */
        .date-selector {
            margin: 30px 0;
            text-align: center;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 15px;
        }
        
        .date-selector label {
            font-weight: bold;
            color: var(--dark-text);
        }
        
        .date-selector input {
            padding: 10px 15px;
            border-radius: 50px;
            border: 2px solid #e0e0e0;
            font-size: 1em;
            transition: all 0.3s;
        }
        
        .date-selector input:focus {
            border-color: var(--primary-color);
            outline: none;
            box-shadow: 0 0 0 3px rgba(52, 152, 219, 0.2);
        }
        
        /* 푸터 */
        footer {
            text-align: center;
            padding: 20px;
            margin-top: 40px;
            color: #777;
            font-size: 0.9em;
        }
        
        /* 애니메이션 */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        /* 반응형 디자인 */
        @media (max-width: 768px) {
            .container {
                padding: 20px;
                margin: 15px;
            }
            
            .button-container {
                flex-direction: column;
                align-items: center;
            }
            
            .link-button {
                width: 100%;
                margin: 5px 0;
            }
            
            .date-selector {
                flex-direction: column;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Nanum+Gothic:wght@400;700&amp;display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <!-- 헤더 -->
    <header>
        <h1 style="color: #ffffff;
    text-align: center;
    margin-bottom: 30px;
    font-size: 2.2em;
">GKS 학교 급식표</h1>
    </header>
    
    <!-- 메인 컨테이너 -->
    <div class="container">
        <!-- 링크 버튼 3개 -->
        <div class="button-container">
            <a href="https://kidongju0000.github.io/el/" class="link-button">
                <i class="fas fa-utensils"></i>
                엘노핌 급식표
            </a>
            <a href="https://kidongju0000.github.io/gr/" class="link-button">
                <i class="fas fa-leaf"></i>
                그린 급식표
            </a>
            <a href="https://kidongju0000.github.io/ms/" class="link-button">
                <i class="fas fa-smile"></i>
                미소 급식표
            </a>
        </div>
        
        <!-- 급식표 섹션 -->
        <div class="meal-section">
            <div class="current-date">2025년 5월 급식표</div>
            
            <table class="meal-table">
                <thead>
                  
                
            </thead></table>
        </div>
    </div>
    
    <!-- 푸터 -->
    <footer>
        <p>© 2023 GKS School. All rights reserved.</p>
        <p>문의: kidongdongju@gmail.com | 전화: 186-2088-5440</p>
    </footer>

</body></html>
