# How to add User Roles & authenticate w Azure using JWT ?

.NET 6 Web API (Create JSON Web Tokens (JWT))
(User Registration / Login / Authentication)

----------------------------------------------------------
1. Add UserDto.cs in App=
   (Username, Password)

2. Add User.cs in App =
   (Username, PasswordHash, PasswordSalt)

3. Add Api Controller-Empty (AuthController.cs) into Controller=
   (Create a method for CreatePasswordHash() method )
   (Create a method for VerifyPasswordHash() method )
   (Create a method to register user/ [HttpPost("register")])
   (Create a method to login user/ [HttpPost("login")]
   (Create a method for CreateToken() method )

4. Add a new section to AppSettings.json=
   (Add "AppSettings"{Token: ...............}.)

5. Add a constructor (public AuthController{IConfiguration ...}) into AuthController.cs
   (Continue to create a method for CreateToken() method )

6. Controll jwt token at jwt.io internet side
----------------------------------------------------------
