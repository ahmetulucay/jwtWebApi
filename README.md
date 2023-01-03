# How to add User Roles & authenticate w Azure using JWT ?

.NET 6 Web API (Create JSON Web Tokens (JWT))
(User Registration / Login / Authentication)
----------------------------------------------------------

![JWTWebApi_Program cs](https://user-images.githubusercontent.com/57094137/210286603-ffd6668d-a7c7-4671-a563-bb31265c6f23.jpg)

1. Add UserDto.cs in App=
   (Username, Password)

![JWTWebApi_User UserDto cs](https://user-images.githubusercontent.com/57094137/210286581-474f6eb8-b630-47a8-9519-b1ab784f378d.jpg)

2. Add User.cs in App =
   (Username, PasswordHash, PasswordSalt)

3. Add Api Controller-Empty (AuthController.cs) into Controller=
 
![JWTWebApi_AuthController cs](https://user-images.githubusercontent.com/57094137/210286791-683bfaf5-b2d1-4819-aec1-8ee6ee65a1fa.jpg)

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
