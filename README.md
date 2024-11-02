<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-image: url('https://i.ibb.co/XVmDd7m/restaurant-image-1.jpg'); /* Background image link */
            background-size: cover;
            background-position: center;
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .login-container {
            background: rgba(255, 255, 255, 0.9);
            padding: 40px;
            width: 100%;
            max-width: 350px;
            text-align: center;
            border-radius: 8px;
            box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.2);
        }

        h2 {
            font-size: 24px;
            color: #333;
            margin-bottom: 20px;
        }

        form {
            display: flex;
            flex-direction: column;
        }

        input[type="email"], input[type="password"] {
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 16px;
        }

        .error-message {
            color: #d9534f;
            font-size: 14px;
            display: none;
        }

        button {
            margin-top: 10px;
            padding: 10px;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }

        .footer-links {
            margin-top: 20px;
            font-size: 14px;
        }

        .footer-links a {
            color: #007bff;
            text-decoration: none;
            margin: 0 5px;
        }

        .footer-links a:hover {
            text-decoration: underline;
        }

        /* Responsive Design */
        @media (max-width: 400px) {
            .login-container {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="login-container">
        <h2>Hello Customer !!</h2>

        <form action="feedback.html" method="POST">
            <input type="email" name="email" placeholder="Email" required>
            <span class="error-message">Invalid Email</span>
            <input type="password" name="password" placeholder="Password" required>
	     <div class="g-recaptcha" data-stekey="6LfLh3AqAAAAAMg5NR_czPRKsQ-pLmgqfo9zGHor"></div>
            <button type="submit">Log In</button>
        </form>
        <div class="footer-links">
            <a href="#">Forgot your password?</a>
            <a href="#">Request an Invite</a>
        </div>
    </div>
</body>
</html>
