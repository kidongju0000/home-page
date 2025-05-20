<html lang="ko"><head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>학교 급식표</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            color: #fff;
            position: relative;
            min-height: 100vh;
        }
        
        /* 배경 이미지 스타일 */
        .background-image {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            z-index: -1;
            opacity: 0.8;
        }
        
        /* 내용을 감싸는 컨테이너 */
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.7);
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
            position: relative;
            margin-top: 50px;
            margin-bottom: 50px;
        }
        
        h1 {
            color: #fff;
            text-align: center;
            margin-bottom: 30px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        
        /* 링크 버튼 컨테이너 */
        .button-container {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }
        
        /* 링크 버튼 스타일 */
        .link-button {
            padding: 12px 25px;
            background-color: #3498db;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: all 0.3s ease;
            margin: 10px;
            text-align: center;
            min-width: 150px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        
        .link-button:hover {
            background-color: #2980b9;
            transform: translateY(-3px);
            box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
        }
        
        /* 급식표 스타일 */
        .meal-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            background-color: rgba(255, 255, 255, 0.9);
            color: #333;
        }
        
        .meal-table th, .meal-table td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: center;
        }
        
        .meal-table th {
            background-color: #3498db;
            color: white;
        }
        
        .meal-table tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        
        .meal-table tr:hover {
            background-color: #e6f7ff;
        }
        
        /* 날짜 선택기 */
        .date-selector {
            margin: 20px 0;
            text-align: center;
        }
        
        .date-selector label {
            font-weight: bold;
            margin-right: 10px;
            color: white;
        }
        
        .date-selector input {
            padding: 8px;
            border-radius: 5px;
            border: none;
        }
        
        @media (max-width: 768px) {
            .button-container {
                flex-direction: column;
                align-items: center;
            }
            
            .link-button {
                width: 80%;
                margin: 5px 0;
            }
        }
    </style>
</head>
<body>
    <!-- 배경 이미지 -->
    <div class="background-image"></div>
    
    <!-- 메인 컨테이너 -->
    <div class="container" style="
    background-color: rgba(0, 0, 0, 1);
    padding-bottom: 47px;
">
        <h1>GKS급식표</h1>
        
        <!-- 링크 버튼 5개 -->
        <div class="button-container">
            <a href="https://www.schoolwebsite.com" class="link-button" target="_blank" style="
    padding-top: 50px;
    padding-bottom: 50px;
">엘노핌</a>
            <a href="https://www.calendar.com" class="link-button" target="_blank" style="
    padding-top: 50px;
">그린</a>
            <a href="https://www.library.com" class="link-button" target="_blank" style="
    padding-top: 50px;
">미소</a>

        </div>
        
        
        
    
    </div>
    


</body></html>
