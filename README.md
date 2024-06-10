# -<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>물건 찾기</title>
    <style>
        .container {
            width: 50%;
            margin: auto;
        }
        .item {
            display: inline-block;
            width: 30%;
            margin: 10px;
            border: 2px solid #ccc; 
            padding: 10px; 
        }
        .item img {
            display: block;
            width: 100%;
            border-radius: 5px; 
        }
        .question {
            margin: 20px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>물건 찾기</h1>
        <div class="items">
            <div class="item" id="gloves">
                <img src="과제용 샂빈/glove.jpeg" alt="장갑">
                <p>장갑</p>
            </div>
            <div class="item" id="camera">
                <img src="과제용 샂빈/ca.jpeg" alt="카메라">
                <p>카메라</p>
            </div>
            <div class="item" id="sunglasses">
                <img src="과제용 샂빈/sunglasses.jpeg" alt="선글라스">
                <p>선글라스</p>
            </div>
            <div class="item" id="tongs">
                <img src="과제용 샂빈/to.jpeg" alt="손톱깎기">
                <p>손톱깎기</p>
            </div>
            <div class="item" id="hairdryer">
                <img src="과제용 샂빈/hair.jpeg" alt="헤어드라이어">
                <p>헤어드라이어</p>
            </div>
            <div class="item" id="bamboo_pillow">
                <img src="과제용 샂빈/bamboo.jpeg" alt="죽부인">
                <p>죽부인</p>
            </div>
        </div>

        <div class="questions">
            <div class="questions">
                <div class="question" id="question1">
                    <p>1. 정호 씨는 열대야로 잠을 못 이루고 있습니다. 시원하게 잠을 자기 위해 필요한 물건은 무엇일까요?</p>
                    <select>
                        <option value="">선택하세요</option>
                        <option value="bamboo_pillow">죽부인</option>
                        <option value="camera">카메라</option>
                        <option value="sunglasses">선글라스</option>
                        <option value="tongs">손톱깎기</option>
                        <option value="hairdryer">헤어드라이어</option>
                        <option value="gloves">장갑</option>
                    </select>
                </div>
                <div class="question" id="question2">
                    <p>2. 준희 씨는 햇빛에 눈이 부셔 운전하기 힘듭니다. 필요한 물건은 무엇일까요?</p>
                    <select>
                        <option value="">선택하세요</option>
                        <option value="sunglasses">선글라스</option>
                        <option value="camera">카메라</option>
                        <option value="bamboo_pillow">죽부인</option>
                        <option value="tongs">손톱깎기</option>
                        <option value="hairdryer">헤어드라이어</option>
                        <option value="gloves">장갑</option>
                    </select>
                </div>
                <div class="question" id="question3">
                    <p>3. 유석 씨는 전망대에 가서 사진을 남기고 싶습니다. 필요한 물건은 무엇일까요?</p>
                    <select>
                        <option value="">선택하세요</option>
                        <option value="camera">카메라</option>
                        <option value="sunglasses">선글라스</option>
                        <option value="bamboo_pillow">죽부인</option>
                        <option value="tongs">손톱깎기</option>
                        <option value="hairdryer">헤어드라이어</option>
                        <option value="gloves">장갑</option>
                    </select>
                </div>
                <div class="question" id="question4">
                    <p>4. 수지 씨 어머니의 손톱이 많이 자랐습니다. 필요한 물건은 무엇일까요?</p>
                    <select>
                        <option value="">선택하세요</option>
                        <option value="tongs">손톱깎기</option>
                        <option value="camera">카메라</option>
                        <option value="sunglasses">선글라스</option>
                        <option value="bamboo_pillow">죽부인</option>
                        <option value="hairdryer">헤어드라이어</option>
                        <option value="gloves">장갑</option>
                    </select>
                </div>
            </div>
            <button onclick="checkAnswers()">확인</button>
        </div>
    </div>

    <script>
        function checkAnswers() {
            const answers = {
                question1: "bamboo_pillow",
                question2: "sunglasses",
                question3: "camera",
                question4: "tongs"
            };

