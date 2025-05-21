<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Login Page</title>
    <link rel="stylesheet" href="style.css" />
    
    <style>
      body {
        font-family: Arial, Helvetica, sans-serif;
        background-image: url("https://media.istockphoto.com/id/1322104312/photo/freedom-chains-that-transform-into-birds-charge-concept.jpg?s=612x612&w=0&k=20&c=e2XUx498GotTLJn_62tPmsqj6vU48ZEkf0auXi6Ywh0=");
        margin: 0;
        padding: 0;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
      }
      .card {
        background: #b2b2b3e1;
        border-radius: 15px;
        padding: 20px;
        width: 500px;
        display: flex;
        flex-direction: column;
        align-items: center;
      }
      h1 {
        text-align: center;
        margin-bottom: 20px;
      }
      form {
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: auto auto auto;
        gap: 10px;
        width: 80%;
      }
      input[type="email"],
      input[type="password"],
      input[type="text"],
      input[type="number"] {
        padding: 10px;
        margin-bottom: 0;
        border: 1px solid #ccc;
        border-radius: 5px;
        width: 100%;
        box-sizing: border-box;
      }
      .full-width {
        grid-column: 1 / 3;
      }
      h1,
      .full-width {
        width: 100%;
        text-align: center;
      }
      .input-group {
        display: flex;
        flex-direction: column;
      }
      input[type="submit"] {
        background-color: #007bff;
        color: white;
        padding: 10px 15px;
        border: none;
        border-radius: 5px;
        cursor: pointer;
      }
      input[type="submit"]:hover {
        background-color: #0056b3;
      }
    </style>
  </head>
  <body>
    
    <div class="card">
      <h1>Log In</h1>
      <form id="loginForm">
        <div class="input-group">
          <input type="email" name="email" id="email" placeholder="Email" />
        </div>
        <div class="input-group">
          <input
            type="password"
            name="password"
            id="password"
            placeholder="Password"
          />
        </div>
        <div class="input-group">
          <input
            type="text"
            name="username"
            id="username"
            placeholder="Username"
          />
        </div>
        <div class="input-group">
          <input
            type="text"
            name="middleName"
            id="middleName"
            placeholder="Middle Name"
          />
        </div>
        <div class="input-group">
          <input
            type="text"
            name="surname"
            id="surname"
            placeholder="Surname"
          />
        </div>
        <div class="input-group">
          <input
            type="number"
            name="phoneNumber"
            id="phoneNumber"
            placeholder="Phone Number"
          />
        </div>
        <input type="submit" value="Log In" class="full-width" />
      </form>
    </div>

    <script>
      document.getElementById('loginForm').addEventListener('submit', function(event) {
        event.preventDefault(); // Prevent the default form submission

        // You can add more sophisticated logic here, like:
        // 1. Getting the values from the input fields:
        //    const email = document.getElementById('email').value;
        //    const password = document.getElementById('password').value;
        //    console.log('Email:', email, 'Password:', password);
        //
        // 2. Sending the data to a server using fetch or XMLHttpRequest.
        //
        // 3. Handling the server's response.

        alert('Form submitted!'); // Basic notification
      });
    </script>
  </body>
</html>
