WSO2 IS Adaptive EmailOTP authenticator. 

Time based two step authentication is where when user tries to login during a specified time period, the user should be allowed to login straight away. And at the rest of the time, the user should be authentication with a second step. Similarly in the role based, only a specific user group should be asked to login with a two step.
As of now till WSO2IS 5.3.0 these adaptive authentication feature is not available as an out-of-the-box feature. But in this authenticator I was able to achieve these scenarios. 

I have taken the Email OTP (One Time Password) authenticator and modified to cater these requirements. So for a given time period the user is able to login with a single step and the remaining time period, the Email OTP is required to login. Also in the same authenticator, it checks the user role and asks the user to login with a two step for that particular role.
