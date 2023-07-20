# kiaSoftTech_project_otpgeneration
This project aims to generate alphanumeric One-Time Passwords (OTPs) using Python. The generated OTPs can be used for various purposes, such as authentication, verification, or password reset mechanisms.
An alphanumeric OTP consists of a combination of letters (both uppercase and lowercase) and digits, making it more secure compared to numeric-only OTPs. This Python project provides a simple OTP generation module that can be easily integrated into other applications.
#CODE
## alphanumeric Otp generation for consule application
import math, random #import librabries
value = "1234567890ABCDEFGHIJKLMNOPQRSTUVWXYZabcdeffghijklmnopqrstuvwxyz" #values which contain in otp
generate_OTP="" #generate otp function
size = 6 #declere size of otp
length=len(value) 
for i in range(size): # range
  generate_OTP+= value[math.floor(random.random() * length)] #takes random values from decleared function 
print(generate_OTP) #calling function with print
