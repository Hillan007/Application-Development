# Application-Development
<!DOCTYPE html>
<html>
<head>
    <title>UniTrade</title>
    <!-- Link to the favicon -->
    <link rel="icon" type="image/png" href="logo.png">
    <!-- Font Awesome CDN -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Boxicons CDN -->
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>

    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
            font-family: Arial, sans-serif;
        }
        #intro {
            position: relative;
            height: 100vh;
            width: 100%;
            overflow: hidden;
        }
        #liveVideo {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: -1;
        }
        .introContent {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: 1;
            text-align: center;
            padding: 0px;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        .highlight {
            background-color: rgba(113, 82, 226, 0.5); /* Semi-transparent black */
            padding: 5px; /* Adjust padding to make the rectangle narrower */
            display: inline-block;
        }
        .welcome-to {
            color: white; /* Set the color for "Welcome to" */
        }
        .uni {
            color: red; /* Set the color for "Uni" */
        }
        .trade {
            color: green; /* Set the color for "Trade" */
        }
        .subtext {
            font-size: 1.2em; /* Smaller than the h1 text */
            color: rgb(248, 227, 227);
        }
        /* New CSS for form styling */
        form {
            display: flex;
            flex-direction: column;
            gap: 5px; /* Reduce space between form elements */
            margin: 10px; /* Reduce margin around the form */
        }

        input[type="text"], input[type="email"], input[type="tel"], input[type="submit"] {
            padding: 5px; /* Reduce padding for form elements */
            margin-top: 5px;
        }

        label {
            font-weight: bold;
        }

        /* New CSS for submit button */
        input[type="submit"] {
            background-color: green; /* Set the background color to green */
            color: white; /* Set the text color to white */
            border: none; /* Remove the border */
            padding: 5px 10px; /* Reduce padding for the submit button */
            cursor: pointer; /* Change the cursor to a pointer on hover */
        }

        input[type="submit"]:hover {
            background-color: darkgreen; /* Change the background color on hover */
        }

        /* New CSS for logo and website name */
        #logoContainer {
            position: absolute;
            top: 10px; /* Adjust top position as needed */
            left: 10%;
            transform: translateX(-50%);
            background-color: rgba(0, 0, 0, 0.5); /* Semi-transparent black */
            padding: 10px;
            border-radius: 5px;
            display: flex;
            align-items: center;
            z-index: 2; /* Ensure it's above other elements */
        }

        #logoContainer img {
            height: 40px; /* Adjust logo height as needed */
            margin-right: 10px;
        }

        #logoContainer span {
            color: white;
            font-size: 15rem; /* Adjust font size as needed */
        }

        /* CSS to make the image circular */
        #circleImage {
            width: 150px; /* Set the desired width */
            height: 150px; /* Set the desired height */
            border-radius: 50%; /* This makes the image circular */
            object-fit: cover; /* Ensures the image covers the entire container */
        }

        /* CSS for social media and phone icons */
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 20px;
        }
        .social-icons a {
            color: black;
            font-size: 24px;
            text-decoration: none;
        }
        .social-icons a:hover {
            color: #209a49; /* Hover color */
        }

        /* CSS for the table and description layout */
        .gallery-item {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        .gallery-item img {
            margin-right: 20px;
        }
        .gallery-description {
            max-width: 600px;
        }

    </style>
