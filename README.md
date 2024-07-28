# Online-Course-Platform
A comprehensive online platform that allows users to browse, view, and enroll in various online courses. Built with Flutter, this application features a user-friendly interface, expert instructors, and a wide range of course offerings in technology, business, personal development, and more.
# code
[6:41 pm, 28/07/2024] Deekshitha.A.R: <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Course Selection</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 600px;
            margin: auto;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            text-align: center;
        }
        label {
            display: block;
            margin-top: 10px;
        }
        select, button {
            width: 100%;
            padding: 10px;
            margin-top: 10px;
        }
        .result {
            margin-top: 20px;
            padding: 10px;
            background-color: #e0ffe0;
            border: 1px solid #b0ffb0;
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Course Selection</h1>
        <form id="courseForm">
            <label for="studentName">Student Name:</label>
            <input type="text" id="studentName" name="studentName" required>

            <label for="courseSelect">Select Course:</label>
            <select id="courseSelect" name="courseSelect" required>
                <option value="" disabled selected>Select your course</option>
                <option value="course1">Course 1</option>
                <option value="course2">Course 2</option>
                <option value="course3">Course 3</option>
                <option value="course4">Course 4</option>
            </select>

            <button type="submit">Submit</button>
        </form>
        <div class="result" id="result"></div>
    </div>

    <script src="app.js"></script>
</body>
</html>
[6:45 pm, 28/07/2024] Deekshitha.A.R: document.getElementById('courseForm').addEventListener('submit', function(event) {
    event.preventDefault();

    var studentName = document.getElementById('studentName').value;
    var courseSelect = document.getElementById('courseSelect').value;

    var resultDiv = document.getElementById('result');
    resultDiv.style.display = 'block';
    resultDiv.textContent = Student ${studentName} has selected ${courseSelect}.;
});
Deekshitha.A.R: import 'package:flutter/material.dart';

