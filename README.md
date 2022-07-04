Program-1: Create an application to design a Visiting Card. The Visiting card should have a company logo at the top right corner. The company name should be displayed in Capital letters, aligned to the center. Information like the name of the employee, job title, phone number, address, email, fax and the website address is to be displayed. Insert a horizontal line between the job title and the phone number. 

1)	Firstly Create an Application by Name “VisitingCardApp” 

2)	Go to xml code of design change the layout to “RelativeLayout” 

3) Add TextView component change the following properties: 
• Size: 38dp 
• Text: DBIT 
• Align left top 

4) Add ImageView to design 
• Download the logo & copy the same in res->drawable folder 
• In xml code of imageview change srcCompat=”@drawable/logo” 
• Align right top 

5) Add View component & change the following properties: 
• Height: 4dp 
• Background: “#4444” (black color) 

6) Add TextView component change the following properties: 
• Size: 20dp 
• Text: Prakruthi S T 
• Style: Bold 
• Align center 

7) Add TextView component change the following properties: 
• Size: 20dp 
• Text: Assistant Professor
• Align center 

8) Add TextView component change the following properties: 
• Size: 20dp 
• Text: Phone-9876543210

9) Add TextView component change the following properties: 
• Size: 20dp 
• Text: Dept. of CSE, DBIT, Bengaluru 
• Align: center 

10) Add TextView component change the following properties: 
• Size: 20dp 
• Text: Email-prakruthit@dbit.co.in 
• Align: center 





 
                   XML-CODE 
<?  xml version="1.0" encoding="utf-8" ?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
tools:context=".MainActivity"> 

<TextView 
android:id="@+id/textView" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginStart="17dp" 
android:layout_marginLeft="17dp" 
android:layout_marginTop="17dp" 
android:layout_marginEnd="244dp" 
android:layout_marginRight="244dp" 
android:layout_marginBottom="486dp" 
android:text="DBIT" 
android:textSize="38dp" /> 

<ImageView 
android:id="@+id/imageView" 
android:layout_width="231dp" 
android:layout_height="174dp" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="-14dp" 
android:layout_marginRight="-14dp" 
android:layout_marginBottom="481dp" 
app:srcCompat="@drawable/dbitlogo" /> 

<View 
android:id="@+id/view" 
android:layout_width="wrap_content" 
android:layout_height="4dp" 
android:layout_alignParentBottom="true" 
android:background="#4444" 
android:layout_marginBottom="466dp" /> 

<TextView 
android:id="@+id/textView2" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="117dp" 
android:layout_marginRight="117dp" 
android:layout_marginBottom="394dp" 
android:text="Prakruthi S T" 
android:textSize="30dp" 
android:textStyle="bold" /> 

<TextView 
android:id="@+id/textView3" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="64dp" 
android:layout_marginRight="64dp" 
android:layout_marginBottom="343dp" 
android:text="Assistant Professor" 
android:textSize="25dp" /> 

<TextView 
android:id="@+id/textView4" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="127dp" 
android:layout_marginRight="127dp" 
android:layout_marginBottom="294dp" 
android:text="Ph No: 9876543210" 
android:textSize="20dp" /> 

<TextView 
android:id="@+id/textView5" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="10dp" 
android:layout_marginRight="10dp" 
android:layout_marginBottom="229dp" 
android:text="Dept. of CSE, DBIT, Bengaluru" 
android:textSize="20dp" /> 

<TextView 
android:id="@+id/textView6" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="44dp" 
android:layout_marginRight="44dp" 
android:layout_marginBottom="189dp" 
android:text="Email: prakruthist@dbit.co.in" 
android:textSize="20dp" /> 
</RelativeLayout> 

JAVA-CODE 
import androidx.appcompat.app.AppCompatActivity; 
import android.os.Bundle; 
public class MainActivity extends AppCompatActivity { 
protected void onCreate(Bundle savedInstanceState) { 
super.onCreate(savedInstanceState); 
setContentView(R.layout.activity_main); 
} 
} 

OUTPUT: 

 
 
 

 🅴🅽🅳
🅴🅽🅳












Program-2: Develop an Android application using controls like Button, TextView, EditText for designing a calculator having basic functionality like Addition, Subtraction, Multiplication, and Division. 

1) Firstly Create an Application by Name “SimpleCalci” 
2) Go to xml code of design change the layout to “RelativeLayout” 
3) Add TextView component & change the following properties: 
• Size: 38dp 
• Text: Simple Calci 
• Center-Align 
4) Add PlainText(EditText) component & change the following properties in XML Code: 
• Text: “” 
• Hint: “Enter the first number” 
• id: “@+id/editText1” 

5) Add PlainText(EditText) component & change the following properties in XML Code: 
• Text: “” 
• Hint: “Enter the second number” 
• id: “@+id/editText2” 
6) Add TextView component to display result & change the following properties: 
• Size: 40dp 
• Text: “0” 
• Center-Align 
• id: “@+id/textView1” 

7) Add 4 Buttons & rename the four buttons “Add”, “Sub”,”Mul” and “div” with following addition: 
• Onclick: “doAdd”(Add Button) 
• Onclick: “doSub”(Sub Button) 
• Onclick: “doMul”(Mul Button) 
• Onclick: “doDiv”(Div Button) 

XML-CODE: 
<?xml version="1.0" encoding="utf-8"?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
tools:context=".MainActivity"> 

<TextView 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="98dp" 
android:layout_marginBottom="653dp" 
android:text="SIMPLE CALCI" 
android:textSize="38dp" 
app:layout_constraintBottom_toBottomOf="parent" 
app:layout_constraintHorizontal_bias="0.498" 
app:layout_constraintLeft_toLeftOf="parent" 
app:layout_constraintRight_toRightOf="parent" 
app:layout_constraintTop_toTopOf="parent" 
app:layout_constraintVertical_bias="0.042" /> 

<EditText 
android:id="@+id/editText1" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="115dp" 
android:layout_marginBottom="547dp" 
android:ems="10" 
android:hint="Enter the First Number" 
android:inputType="textPersonName" 
android:text="" /> 

<EditText 
android:id="@+id/editText2" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="111dp" 
android:layout_marginBottom="455dp" 
android:ems="10" 
android:inputType="textPersonName" 
android:hint="Enter the Second Number" 
android:text="" /> 

<TextView 
android:id="@+id/textView1" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="203dp" 
android:layout_marginBottom="350dp" 
android:text="0" 
android:textSize="40dp" /> 

<Button 
android:id="@+id/button" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="274dp" 
android:layout_marginBottom="237dp" 
android:onClick="doAdd" 
android:text="ADD" /> 

<Button 
android:id="@+id/button2" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="68dp" 
android:layout_marginBottom="233dp" 
android:onClick="doSub" 
android:text="SUB" /> 

<Button 
android:id="@+id/button3" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="277dp" 
android:layout_marginBottom="115dp" 
android:onClick="doMul" 
android:text="MUL" /> 

<Button 
android:id="@+id/button4" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="63dp" 
android:layout_marginBottom="104dp" 
android:onClick="doDiv" 
android:text="DIV" /> 

</RelativeLayout> 

JAVA-CODE: 

import androidx.appcompat.app.AppCompatActivity; 
import android.os.Bundle; 
import android.view.View; 
import android.widget.EditText; 
import android.widget.TextView; 

public class MainActivity extends AppCompatActivity { 
EditText e1,e2; 
TextView tv1; 
@Override 
protected void onCreate(Bundle savedInstanceState) { 
super.onCreate(savedInstanceState); 
setContentView(R.layout.activity_main); 
e1 = (EditText)findViewById(R.id.editText1); 
e2 = (EditText)findViewById(R.id.editText2); 
tv1 = (TextView)findViewById(R.id.textView1); 
} 
public void doAdd(View V){ 
int a1 = Integer.parseInt(e1.getText().toString()); 
int a2 = Integer.parseInt(e2.getText().toString()); 
int result= a1+a2; 
tv1.setText(""+result); 
} 
public void doSub(View V){ 
int a1 = Integer.parseInt(e1.getText().toString()); 
int a2 = Integer.parseInt(e2.getText().toString()); 
int result= a1-a2; 
tv1.setText(""+result); 
} 
public void doMul(View V){ 
int a1 = Integer.parseInt(e1.getText().toString()); 
int a2 = Integer.parseInt(e2.getText().toString()); 
int result= a1*a2; 
tv1.setText(""+result); 
} 
public void doDiv(View V){ 
int a1 = Integer.parseInt(e1.getText().toString()); 
int a2 = Integer.parseInt(e2.getText().toString()); 
float result= a1/a2; 
tv1.setText(""+result); 
} 
} 
OUTPUT: 
 
 	 


 🅴🅽🅳
🅴🅽🅳








Program-3: Create a SIGN Up activity with Username and Password. Validation of password should happen based on the following rules: 
• Password should contain uppercase and lowercase letters. 
• Password should contain letters and numbers. 
• Password should contain special characters. 
• Minimum length of the password (the default value is 8). 
On successful SIGN UP proceed to the next Login activity. Here the user should SIGN IN   using the Username and Password created during signup activity. If the Username and Password are matched then navigate to the next activity which displays a message saying “Successful Login” or else display a toast message saying  “Login Failed”. The user is given only two attempts and after that display a toast message saying “Failed Login Attempts” and disable the SIGN IN button. Use Bundle to transfer information from one activity to another. 

1)	Go to xml code of design Firstly Create an Application by Name “SignUpActivity” 

2)	change the layout to “RelativeLayout” 

3) Add TextView component & change the following properties: 
• Size: 38dp 
• Text: “Sign Up” 
• Center-Align 

4) Add Email (EditText) component & change the following properties in XML Code: 
• Hint: “Email ID” 
• id: “@+id/emailEditText” 

5) Add Password (EditText) component & change the following properties in XML 
Code: 
• Hint: “Password” 
• id: “@+id/passwordEditText” 

6) Add Button component & change the following properties in XML 
• Id: “@+id/signBtn” 
• Text: “Sign Up” 

XML-CODE 
<?xml version="1.0" encoding="utf-8"?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
tools:context=".MainActivity"> 
<TextView 
android:layout_width="160dp" 
android:layout_height="42dp" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="112dp" 
android:layout_marginBottom="573dp" 
android:text="Sign Up" 
android:textSize="28dp" 
app:layout_constraintBottom_toBottomOf="parent" 
app:layout_constraintLeft_toLeftOf="parent" 
app:layout_constraintRight_toRightOf="parent" 
app:layout_constraintTop_toTopOf="parent" /> 

<EditText 
android:id="@+id/emailEditText" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="29dp" 
android:layout_marginBottom="431dp" 
android:ems="10" 
android:hint="Email ID" 
android:inputType="textEmailAddress" 
android:textSize="28dp" /> 

<EditText 
android:id="@+id/passwordEditText" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="34dp" 
android:layout_marginBottom="345dp" 
android:ems="10" 
android:hint="Password" 
android:inputType="textPassword" 
android:textSize="28dp" /> 

<Button 
android:id="@+id/signUpBtn" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="106dp" 
android:layout_marginBottom="226dp" 
android:text="Sign Up" 
android:textSize="28dp" /> 

</RelativeLayout> 

 
 JAVA-CODE 
package com.example.loginapplication; 
import androidx.appcompat.app.AppCompatActivity; 
import android.content.Intent; 
import android.os.Bundle; 
import android.view.View; 
import android.widget.Button; 
import android.widget.EditText; 
import android.widget.Toast; 
import java.util.regex.Pattern; 
public class MainActivity extends AppCompatActivity { 
EditText emailEditText, passwordEditText; 
Button signUpBtn; 
@Override 
protected void onCreate(Bundle savedInstanceState) { 
super.onCreate(savedInstanceState); 
setContentView(R.layout.activity_main); 
emailEditText = findViewById(R.id.emailEditText); 
passwordEditText = findViewById(R.id.passwordEditText); 
signUpBtn = findViewById(R.id.signUpBtn); 
signUpBtn.setOnClickListener(new View.OnClickListener() { 
@Override 
public void onClick(View v) { 
String email = emailEditText.getText().toString(); 
String password = passwordEditText.getText().toString(); 
if (!isValidPassword(password)) { 
Toast.makeText(MainActivity.this, "Password Does not match the rules", Toast.LENGTH_LONG).show(); 
return; 
} 
Intent intent = new Intent(MainActivity.this, LoginActivity.class); 
intent.putExtra("email", email); 
intent.putExtra("password", password); 
startActivity(intent); 
} 
}); 
} 
Pattern lowercase = Pattern.compile("^.*[a-z].*$"); 
Pattern uppercase = Pattern.compile("^.*[A-Z].*$"); 
Pattern number = Pattern.compile("^.*[0-9].*$"); 
Pattern specialCharacter = Pattern.compile("^.*[^a-zA-Z0-9].*$"); 

 private Boolean isValidPassword(String password) { 
if (password.length() < 8) { 
return false; 
} 
if (!lowercase.matcher(password).matches()) { 
return false; 
} 
if (!uppercase.matcher(password).matches()) { 
return false; 
} 
if (!number.matcher(password).matches()) { 
return false; 
} 
if (!specialCharacter.matcher(password).matches()) { 
return false; 
} 
return true; 
} 
} 

7) Right click on Java folder-> new-> activity->empty activity-> name it as 
“LoginActivity” 
8) Go to xml code of design change the layout to “RelativeLayout” 
9) Add TextView component & change the following properties: 
• Size: 38dp 
• Text: “Login” 
• Center-Align 
10) Add Email (EditText) component & change the following properties in XML Code: 
• Hint: “Email ID” 
• id: “@+id/emailEditText” 

11) Add Password (EditText) component & change the following properties in XML 
Code: 
• Hint: “Password” 
• id: “@+id/passwordEditText” 
12) Add Button component & change the following properties in XML 
• Id: “@+id/loginBtn” 
• Text: “Login” 
XML-CODE 
<?xml version="1.0" encoding="utf-8"?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
tools:context=".LoginActivity"> 

<TextView 
android:id="@+id/textView" 
android:layout_width="210dp" 
android:layout_height="54dp" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="120dp" 
android:layout_marginBottom="576dp" 
android:text="Login Activity" 
android:textSize="28dp" /> 

<EditText 
android:id="@+id/emailEditText" 
android:layout_width="222dp" 
android:layout_height="80dp" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="108dp" 
android:layout_marginBottom="424dp" 
android:ems="10" 
android:hint="Email ID" 
android:inputType="textEmailAddress" 
android:textSize="28dp" /> 

<EditText 
android:id="@+id/passwordEditText" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="40dp" 
android:layout_marginBottom="299dp" 
android:ems="10" 
android:hint="Password" 
android:inputType="textPassword" 
android:textSize="28dp" /> 

<Button 
android:id="@+id/loginBtn" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="173dp" 
android:layout_marginBottom="189dp" 
android:text="login" 
android:textSize="26dp" /> 

</RelativeLayout> 

JAVA-CODE 
package com.example.loginapplication; 
import androidx.appcompat.app.AppCompatActivity; 

import android.content.Intent; 
import android.os.Bundle; 
import android.view.View; 
import android.widget.Button; 
import android.widget.EditText; 
import android.widget.Toast; 
public class LoginActivity extends AppCompatActivity { 
EditText emailEditText, passwordEditText; 
Button loginBtn; 
int counter=2; 
@Override 
protected void onCreate(Bundle savedInstanceState) { 
super.onCreate(savedInstanceState); 
setContentView(R.layout.activity_login); 
emailEditText=findViewById(R.id.emailEditText); 
passwordEditText=findViewById(R.id.passwordEditText); 
loginBtn=findViewById(R.id.loginBtn); 
String registeredEmail=getIntent().getStringExtra("email"); 
String registeredPassword=getIntent().getStringExtra("password"); 
loginBtn.setOnClickListener(new View.OnClickListener() { 
@Override 
public void onClick(View v) { 
String email=emailEditText.getText().toString(); 
String password=passwordEditText.getText().toString(); 
if(registeredEmail.equals(email)&& registeredPassword.equals(password)) 
{ 
Intent intent=new Intent(LoginActivity.this,LoginSuccessActivity.class); 
startActivity(intent); 
} 
else{ 
Toast.makeText(LoginActivity.this,"Invalid 
Credentials",Toast.LENGTH_LONG).show(); 
} 
counter--; 
if (counter==0) 
{ 
Toast.makeText(getBaseContext(),"FAILED LOGIN 
ATTEMPTS",Toast.LENGTH_LONG).show(); 
loginBtn.setEnabled(false); 
} 
} 
}); 
} 
} 
 
13) Right click on Java folder-> new-> activity->empty activity-> name it as 
“LoginSuccessful” 

14) Go to xml code of design change the layout to “RelativeLayout” 

15) Add TextView component & change the following properties: 
• Size: 38dp 
• Text: “Login Successful” 
• Center-Align 

XML-CODE 
<?xml version="1.0" encoding="utf-8"?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
tools:context=".LoginSuccessActivity"> 

<TextView 
android:id="@+id/textView2" 
android:layout_width="297dp" 
android:layout_height="190dp" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="42dp" 
android:layout_marginBottom="400dp" 
android:text="Login Successful" 
android:textSize="38dp" /> 

</RelativeLayout> 
 
JAVA-CODE 
package com.example.loginapplication; 
import androidx.appcompat.app.AppCompatActivity; 
import android.os.Bundle; 
public class LoginSuccessActivity extends AppCompatActivity { 
@Override 
protected void onCreate(Bundle savedInstanceState) { 
super.onCreate(savedInstanceState); 
setContentView(R.layout.activity_login_success); 
} 
} 
 






OUTPUT 

 	 	 

 
 
 
 
 
 
 
 
 
 
 
 
🅴🅽🅳
🅴🅽🅳











 
Program-4: Develop an application to set an image as wallpaper. On click of a button, the wallpaper image should start to change randomly every 30 seconds. 

1)	Firstly Create an Application by Name “WallpaperActivity” 

2)	Go to xml code of design change the layout to “RelativeLayout” 

3) Add TextView component & change the following properties: 
• Size: 38dp 
• Text: Wall Paper Change Application 
• Center-Align 

4) Add Button component & change the following properties: 
• Size: 38dp 
• Text: Click Here To Change Wall Paper
 
5) Save five images (jpg format) in the drawable folder. In this example one.jpg, two.jpg, three.jpg, four.jpg and five.jpg images are saved in drawable folder. 

XML-CODE 
<?xml version="1.0" encoding="utf-8"?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
tools:context=".MainActivity"> 

<TextView 
android:id="@+id/textView" 
android:layout_width="210dp" 
android:layout_height="54dp" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="120dp" 
android:layout_marginBottom="576dp" 
android:text="Wall Paper Change Application" 
android:textSize="28dp" /> 

<Button 
android:id="@+id/button" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="173dp" 
android:layout_marginBottom="189dp" 
android:text="Click Here To Change Wall Paper" 
android:textSize="26dp" /> 
</RelativeLayout> 

 



 
JAVA-CODE 
import androidx.appcompat.app.AppCompatActivity; 
import android.app.WallpaperManager; 
import android.graphics.Bitmap; 
import android.graphics.BitmapFactory; 
import android.graphics.drawable.AnimationDrawable; 
import android.graphics.drawable.BitmapDrawable; 
import android.graphics.drawable.Drawable; 
import android.os.Bundle; 
import android.view.View; 
import android.widget.Button; 
import android.widget.Toast; 
import java.io.IOException; 
import java.util.Timer; 
import java.util.TimerTask; 

public class MainActivity extends AppCompatActivity { 
Button changewallpaper; 
Timer mytimer; 
Drawable drawable; 
WallpaperManager wpm; 

int prev=1; 

@Override 
protected void onCreate(Bundle savedInstanceState) { 
super.onCreate(savedInstanceState); 
setContentView(R.layout.activity_main); 
mytimer = new Timer(); 
wpm = WallpaperManager.getInstance(this); 
changewallpaper = findViewById(R.id.button); 
changewallpaper.setOnClickListener(new View.OnClickListener() { 
@Override public void onClick(View view) { 
setWallpaper(); 
} 
}); 
} 
private void setWallpaper() { 
mytimer.schedule(new TimerTask() { 
@Override 
public void run() { 
if(prev==1) { 
drawable = getResources().getDrawable(R.drawable.one); 
prev = 2; 
} 
else if(prev==2) { 
drawable = getResources().getDrawable(R.drawable.two); 
prev=3; 
} 
else if(prev==3) { 
drawable = getResources().getDrawable(R.drawable.three); 
prev=4; 
} 
else if(prev==4) { 
drawable = getResources().getDrawable(R.drawable.four); 
prev=5; 
} 
else if(prev==5) { 
drawable = getResources().getDrawable(R.drawable.five); 
prev=1; 
} 
Bitmap wallpaper = ((BitmapDrawable)drawable).getBitmap(); 
try { 
wpm.setBitmap(wallpaper); 
} catch (IOException e) { 
e.printStackTrace(); 
} 
} 
},0,30000); } } 

Output: 
 
 

 
 	 	 













Program-5 : Write a program to create an activity with two buttons START and STOP. On pressing of the START button, the activity must start the counter by displaying the numbers from One and the counter must keep on counting until the STOP button is pressed. Display the counter value in a TextViewcontrol. 

1)	Firstly Create an Application by Name “CounterActivity”

2)	Go to xml code of design change the layout to “RelativeLayout” 

3) Add TextView component & change the following properties: 
• Size: 38dp 
• Text: “Counter Application” 
• Center-Align 

4) Add TextView component & change the following properties: 
• Text: “Counter Value” 

5) Add Button components & change the following properties: 
• Size: 38dp 
• Text: Start 
• id: “@+id/btn_start” 

6) Add Button components & change the following properties: 
• Size: 38dp 
• Text: Stop 
• id: “@+id/btn_stop” 

XML-CODE 

<?xml version="1.0" encoding="utf-8"?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
tools:context=".MainActivity"> 

<TextView 
android:layout_width="378dp" 
android:layout_height="68dp" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="18dp" 
android:layout_marginBottom="602dp" 
android:text="Counter Application" 
android:textSize="38dp" 
app:layout_constraintBottom_toBottomOf="parent" 
app:layout_constraintLeft_toLeftOf="parent" 
app:layout_constraintRight_toRightOf="parent" 
app:layout_constraintTop_toTopOf="parent" /> 

<TextView 
android:id="@+id/textView" 
 android:layout_width="121dp" 
android:layout_height="32dp" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="145dp" 
android:layout_marginBottom="478dp" 
android:text="Counter Value" /> 

<Button 
android:id="@+id/btn_start" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="297dp" 
android:layout_marginBottom="295dp" 
android:text="Start" /> 

<Button 
android:id="@+id/btn_stop" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="74dp" 
android:layout_marginBottom="292dp" 
android:text="Stop" /> 

</RelativeLayout> 
 
JAVA-CODE 
package com.example.counterapplication; 
import androidx.appcompat.app.AppCompatActivity; 
import android.os.Bundle; 
import android.os.Handler; 
import android.view.View; 
import android.widget.Button; 
import android.widget.TextView; 

public class MainActivity extends AppCompatActivity { 
Button btnstart, btnstop; 
TextView txtcounter; 
int i=1; 
Handler customHandler=new Handler(); 
@Override 

protected void onCreate(Bundle savedInstanceState) { 
super.onCreate(savedInstanceState); 
setContentView(R.layout.activity_main); 
btnstart=findViewById(R.id.btn_start); 
btnstop=findViewById(R.id.btn_stop); 
txtcounter=findViewById(R.id.textView); 
btnstart.setOnClickListener(new View.OnClickListener() { 
@Override 
public void onClick(View v) { 
customHandler.postDelayed(updateTimerThread,0); 
} 
}); 

btnstop.setOnClickListener(new View.OnClickListener() { 
@Override 
public void onClick(View v) { 
customHandler.removeCallbacks(updateTimerThread); 
} 
}); 
} 
private final Runnable updateTimerThread=new Runnable() { 
@Override 
public void run() { 
txtcounter.setText(""+i); 
customHandler.postDelayed(this,1000); 
i++; 
} 
}; 
} 

Output: 
 
 
🅴🅽🅳
🅴🅽🅳
🅴🅽🅳
 	 



Program-6: Create two files of XML and JSON type with values for City_Name, Latitude, Longitude, Temperature, and Humidity. Develop an application to create an activity with two buttons to parse the XML and JSON files which when clicked should display the data in their respective layouts side by side. 
 
1)	Firstly Create an Application by Name “JsonParser” 

2)	Go to xml code of design change the layout to “RelativeLayout” 

3) Add TextView component & change the following properties: 
1) Size: 38dp 
2) Text: XML and JSON Parser 
3) Center-Align 
4) Add Two Buttons to Design & change the name “ParseXml” & “ParseJson” with following onclick functions: 
• ParseXml-Button: parsexml 
• ParseJson-Button: parsejson 

5) Add TextView component & change the following properties: 
• Id: display 
• Text: “” 
• Align: Center 

6) Add Assets folder by following the given hierarchy: 
App->new->folder->Assests folder 

7) Inside the assets folder create new files of xml and json using the following hierarchy: new->file->city.xml 
new->file->city.json 
once created place the following details inside the “city.xml” and “city.json” 

 city.xml Code :
<?xml version="1.0" encoding="utf-8"?>
<place>
 <city>
 <name>Bangalore</name>
 <longitude >16.4567</longitude>
 <latitude>18.685347</latitude>
 <temperature>22</temperature>
 <humidity>93%</humidity>
 </city>
</place>











 city.json Code :
{
 "place":[
 {
 "name": " Bangalore ",
 "longitude":16.4567,
 "latitude":18.685347,
 "temperature":22,
 "humidity":"93%" 
} 
]
}

XML-CODE: 
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentStart="true"
        android:layout_alignParentLeft="true"
        android:layout_alignParentTop="true"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="109dp"
        android:layout_marginLeft="109dp"
        android:layout_marginTop="62dp"
        android:text="PARSE XML and JSON FILES" />

    <Button
        android:id="@+id/parseXmlBtn"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="133dp"
        android:text="PARSE XML"
        android:onClick="parsexml"/>

    <Button
        android:id="@+id/parseJsonBtn"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="218dp"
        android:text="PARSE JSON"
        android:onClick="parsejson"/>

    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentStart="true"
        android:layout_alignParentLeft="true"
        android:layout_alignParentTop="true"
        android:layout_marginStart="16dp"
        android:layout_marginLeft="16dp"
        android:layout_marginTop="304dp"
        android:text="Parsed XML File Data" />

    <TextView
        android:id="@+id/textView3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_marginTop="301dp"
        android:layout_marginEnd="21dp"
        android:layout_marginRight="21dp"
        android:text="Parsed JSON File Data" />

    <TextView
        android:id="@+id/displayTextView"
        android:layout_width="154dp"
        android:layout_height="216dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentLeft="true"
        android:layout_alignParentBottom="true"
        android:layout_marginStart="15dp"
        android:layout_marginLeft="15dp"
        android:layout_marginBottom="163dp"
        android:text="" />

    <TextView
        android:id="@+id/displayTextView1"
        android:layout_width="154dp"
        android:layout_height="216dp"
        android:layout_alignParentStart="true"
        android:layout_alignParentLeft="true"
        android:layout_alignParentBottom="true"
        android:layout_marginStart="237dp"
        android:layout_marginLeft="237dp"
        android:layout_marginBottom="159dp"
        android:text="" />


</RelativeLayout>

JAVA-CODE: 
package com.example.xmlandjsonfiledisplay;
import androidx.annotation.RequiresApi;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Build;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.TextView;
import android.widget.Toast;
import org.json.JSONArray;
import org.json.JSONException;
import org.json.JSONObject;
import org.w3c.dom.Document;
import org.w3c.dom.Element;
import org.w3c.dom.Node;
import org.w3c.dom.NodeList;
import java.io.IOException;
import java.io.InputStream;
import java.nio.charset.StandardCharsets;
import javax.xml.parsers.DocumentBuilder;
import javax.xml.parsers.DocumentBuilderFactory;
public class MainActivity extends AppCompatActivity {
    Button parseXmlBtn, parseJsonBtn;
    TextView t1,t2;
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        parseJsonBtn = findViewById(R.id.parseJsonBtn);
        parseXmlBtn = findViewById(R.id.parseXmlBtn);
        t1 = findViewById(R.id.displayTextView);
        t2 = findViewById(R.id.displayTextView1);
    }
    public void parsexml(View v) {
        try {
            InputStream is = getAssets().open("City.xml");
            DocumentBuilderFactory documentBuilderFactory =DocumentBuilderFactory.newInstance(); //API to get the parser that produces DOM tree from XML document
            DocumentBuilder documentBuilder = documentBuilderFactory.newDocumentBuilder(); //API to obtain DOM document instance from XML document
            Document document = documentBuilder.parse(is);
            Element element=document .getDocumentElement();
            element.normalize();
            StringBuilder stringBuilder = new StringBuilder();
            stringBuilder.append("XML Data");
            stringBuilder.append("\n----------");
            NodeList nodeList = document.getElementsByTagName("city");
            for (int i = 0; i < nodeList.getLength(); i++) {
                Node node = nodeList.item(i);
                if (node.getNodeType() == Node.ELEMENT_NODE) {
                    stringBuilder.append("\nName: ").append(getValue("name", element));
                    stringBuilder.append("\nLatitude: ").append(getValue("latitude", element));
                    stringBuilder.append("\nLongitude: ").append(getValue("longitude", element));
                    stringBuilder.append("\nTemperature: ").append(getValue("temperature", element));
                    stringBuilder.append("\nHumidity: ").append(getValue("humidity", element));
                    stringBuilder.append("\n----------");
                }
            }
            t1.setText(stringBuilder.toString());
            is.close();
        } catch (Exception e) {
            e.printStackTrace();
            Toast.makeText(MainActivity.this, "Error Parsing XML",
                    Toast.LENGTH_SHORT).show();
        }
    }
    @RequiresApi(api = Build.VERSION_CODES.KITKAT)
    public void parsejson(View v) {
        String json;
        StringBuilder stringBuilder = new StringBuilder();
        try {
            InputStream is = getAssets().open("City.json");
            int size = is.available(); // estimates the number of bytes that can be read from input stream
            byte[] buffer = new byte[size];
            is.read(buffer);
            json = new String(buffer, StandardCharsets.UTF_8);
            JSONObject obj=new JSONObject (json);
            JSONArray jsonArray = obj.optJSONArray("place");
            stringBuilder.append("JSON Data");
            stringBuilder.append("\n----------");
            for (int i = 0; i < jsonArray.length(); i++) {
                JSONObject jsonObject = jsonArray.getJSONObject(i);
                stringBuilder.append("\nName: ").append(jsonObject.getString("name"));
                stringBuilder.append("\nLatitude: ").append(jsonObject.getString("latitude"));
                stringBuilder.append("\nLongitude: ").append(jsonObject.getString("longitude"));
                stringBuilder.append("\nTemperature: ").append(jsonObject.getString("temperature"));
                stringBuilder.append("\nHumidity: ").append(jsonObject.getString("humidity"));
                stringBuilder.append("\n----------");
            }
            t2.setText(stringBuilder.toString());
            is.close();
        } catch (IOException | JSONException e) {
            e.printStackTrace();
            Toast.makeText(MainActivity.this, "Error in parsing JSON data from json file!",Toast.LENGTH_SHORT).show();
        }
    }
    private static String getValue(String tag,Element element)
    {
        NodeList nodeList=element.getElementsByTagName(tag).item(0).getChildNodes();
        Node node=(Node)nodeList.item(0);
        return node.getNodeValue();
    }
}

















OUTPUT: 
 
 	 	 

 🅴🅽🅳🅴🅽🅳

🅴🅽🅳
🅴🅽🅳
🅴🅽🅳
🅴🅽🅳

 
 
 
 
 







Program-7: Develop a simple application with one EditText so that the user can write some text in it. Create a button called “Convert Text to Speech” that converts the user input text into voice.
 
1)	Firstly Create an Application by Name “TextToSpeech” 

2)	Go to xml code of design change the layout to “RelativeLayout” 


3)	Add TextView component & change the following properties: 

•	Size: 38dp 
•	Text: Text2Speech App 
•	Center-Align 

4) Add PlainText(EditText) component & change the following properties in XML 
Code: 
• Text: “” 
• Hint: “Enter the text to be converted” 
• id: “@+id/editText” 

8) Add Button component & change the following properties in XML Code: 
• Name: Convert 
• onClick: convert 

XML-CODE: 
<?xml version="1.0" encoding="utf-8"?> 
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android" 
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
tools:context=".MainActivity"> 

<TextView 
android:id="@+id/textView" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="59dp" 
android:layout_marginRight="59dp" 
android:layout_marginBottom="649dp" 
android:text="Text2SpeechApp" 
android:textSize="40dp" /> 

<EditText 
android:id="@+id/editText" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="101dp" 
android:layout_marginRight="101dp" 
android:layout_marginBottom="514dp" 
android:ems="10" 
android:hint="Enter the text to be converted" 
android:inputType="textPersonName" 
android:text="" /> 

<Button 
android:id="@+id/button" 
android:layout_width="wrap_content" 
android:layout_height="wrap_content" 
android:layout_alignParentEnd="true" 
android:layout_alignParentRight="true" 
android:layout_alignParentBottom="true" 
android:layout_marginEnd="162dp" 
android:onClick="convert" 
android:layout_marginRight="162dp" 
android:layout_marginBottom="329dp" 
android:text="Convert" /> 
</RelativeLayout> 

JAVA-CODE: 
import androidx.appcompat.app.AppCompatActivity; 
import android.os.Bundle; 
import android.speech.tts.TextToSpeech; 
import android.view.View; 
import android.widget.EditText; 
import android.widget.Toast; 

import java.util.Locale; 
public class MainActivity extends AppCompatActivity { 
TextToSpeech t1; 
EditText e1; 
@Override 
protected void onCreate(Bundle savedInstanceState) { 
super.onCreate(savedInstanceState); 
setContentView(R.layout.activity_main); 
e1 = findViewById(R.id.editText); 
t1 = new TextToSpeech(getApplicationContext(), new 
TextToSpeech.OnInitListener() { 
@Override 
public void onInit(int status) { 
if (status!=TextToSpeech.ERROR){ 
t1.setLanguage(Locale.UK); 
} 
                } 
}); 
} 
public void convert(View view){ 
String tospeak = e1.getText().toString(); 
t1.speak(tospeak,TextToSpeech.QUEUE_FLUSH,null); 
} 
} 




OUTPUT: 
 
 
 
 
 
 
 
 
 🅴🅽🅳
🅴🅽🅳
🅴🅽🅳

 














 
Program-8: Create an activity like a phone dialer with CALL and SAVE buttons. On pressing the CALL button, it must call the phone number and on pressing the SAVE 
button it must save the number to the phone contacts. 

1)	Firstly Create an Application by Name “CallActivity” 

2)	Go to xml code of design change the layout to “RelativeLayout” 

3) Add TextView component & change the following properties: 
• Size: 38dp 
• Text: Call Activity 
• Center-Align 

4) Add EditText component & change the following properties in XML Code: 
• id: “@+id/phoneNumberEditText” 

5) Add PlainText(EditText) component & change the following properties in XML Code: 
• Text: “” 
• Hint: “Copied Text” 
• id: “@+id/editText2” 

6) Add three buttons to the design & change the text of the Buttons to “Clear”, “Call”, “Save” and change the id as follows: 
• id:”@+id/clearBtn” 
• id:”@+id/callBtn” 
• id:”@+id/saveBtn” 

7) Add twelve buttons to the design & change the text of the Buttons as 1,2,3,4,5,6,7,8,9,0,*,# 

XML-CODE 
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto"
xmlns:tools="http://schemas.android.com/tools"
android:layout_width="match_parent"
android:layout_height="match_parent"
tools:context=".MainActivity">

    <TextView
        android:layout_width="298dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_centerHorizontal="true"
        android:layout_marginEnd="56dp"
        android:layout_marginRight="56dp"
        android:layout_marginBottom="656dp"
        android:text="Call Application"
        android:textSize="36dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <EditText
        android:id="@+id/phoneNumberEditText"
        android:layout_width="262dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_centerHorizontal="true"
        android:layout_marginEnd="123dp"
        android:layout_marginRight="123dp"
        android:layout_marginBottom="571dp"
        android:ems="10"
        android:inputType="phone" />

    <Button
        android:id="@+id/clearBtn"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_marginEnd="16dp"
        android:layout_marginRight="16dp"
        android:layout_marginBottom="573dp"
        android:text="Clear" />

    <Button
        android:id="@+id/button2"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_marginEnd="288dp"
        android:layout_marginRight="288dp"
        android:layout_marginBottom="458dp"
        android:onClick="inputNumber"
        android:text="1" />

    <Button
        android:id="@+id/button3"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_centerHorizontal="true"
        android:layout_marginEnd="168dp"
        android:layout_marginRight="168dp"
        android:layout_marginBottom="456dp"
        android:onClick="inputNumber"
        android:text="2" />

    <Button
        android:id="@+id/button4"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_marginEnd="55dp"
        android:layout_marginRight="55dp"
        android:layout_marginBottom="457dp"
        android:onClick="inputNumber"
        android:text="3" />

    <Button
        android:id="@+id/button5"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_marginEnd="286dp"
        android:layout_marginRight="286dp"
        android:layout_marginBottom="378dp"
        android:onClick="inputNumber"
        android:text="4" />

    <Button
        android:id="@+id/button6"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_centerHorizontal="true"
        android:layout_marginEnd="169dp"
        android:layout_marginRight="169dp"
        android:layout_marginBottom="367dp"
        android:onClick="inputNumber"
        android:text="5" />

    <Button
        android:id="@+id/button7"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_marginEnd="54dp"
        android:layout_marginRight="54dp"
        android:layout_marginBottom="363dp"
        android:onClick="inputNumber"
        android:text="6" />

    <Button
        android:id="@+id/button8"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_centerVertical="true"
        android:layout_marginEnd="290dp"
        android:layout_marginRight="290dp"
        android:layout_marginBottom="294dp"
        android:onClick="inputNumber"
        android:text="7" />

    <Button
        android:id="@+id/button9"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_centerInParent="true"
        android:layout_marginEnd="169dp"
        android:layout_marginRight="169dp"
        android:layout_marginBottom="291dp"
        android:onClick="inputNumber"
        android:text="8" />

    <Button
        android:id="@+id/button10"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_centerVertical="true"
        android:layout_marginEnd="57dp"
        android:layout_marginRight="57dp"
        android:layout_marginBottom="290dp"
        android:onClick="inputNumber"
        android:text="9" />

    <Button
        android:id="@+id/button11"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_marginEnd="293dp"
        android:layout_marginRight="293dp"
        android:layout_marginBottom="216dp"
        android:onClick="inputNumber"
        android:text="#" />

    <Button
        android:id="@+id/button12"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_centerHorizontal="true"
        android:layout_marginEnd="171dp"
        android:layout_marginRight="171dp"
        android:layout_marginBottom="213dp"
        android:onClick="inputNumber"
        android:text="0" />

    <Button
        android:id="@+id/button13"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_marginEnd="57dp"
        android:layout_marginRight="57dp"
        android:layout_marginBottom="214dp"
        android:onClick="inputNumber"
        android:text="*" />

    <Button
        android:id="@+id/callBtn"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_marginEnd="229dp"
        android:layout_marginRight="229dp"
        android:layout_marginBottom="123dp"
        android:text="Call" />

    <Button
        android:id="@+id/saveBtn"
        android:layout_width="76dp"
        android:layout_height="wrap_content"
        android:layout_alignParentEnd="true"
        android:layout_alignParentRight="true"
        android:layout_alignParentBottom="true"
        android:layout_centerHorizontal="true"
        android:layout_marginEnd="115dp"
        android:layout_marginRight="115dp"
        android:layout_marginBottom="128dp"
        android:text="Save" />
</RelativeLayout>
 
 
JAVA-CODE 
package com.example.callingapplication; 
package com.example.callandsaveapp;
import androidx.appcompat.app.AppCompatActivity;
import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.provider.ContactsContract;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
public class MainActivity extends AppCompatActivity {
    EditText phoneNumberEditText;
    Button clearBtn,callBtn,saveBtn;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        phoneNumberEditText=findViewById(R.id.phoneNumberEditText);
        callBtn=findViewById(R.id.callBtn);
        saveBtn=findViewById(R.id.saveBtn);
        clearBtn=findViewById(R.id.clearBtn);

        clearBtn.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                phoneNumberEditText.setText("");
            }
        });
        callBtn.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                String phoneNumber=phoneNumberEditText.getText().toString();
                Intent intent=new Intent(Intent.ACTION_DIAL); //it triggers the built in phone call functionality
                intent.setData(Uri.parse("tel:"+phoneNumber));
                startActivity(intent);
            }
        });
        saveBtn.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                String phoneNumber=phoneNumberEditText.getText().toString();
                Intent intent=new Intent(Intent.ACTION_INSERT); //insert an empty item to the given intent
                intent.setType(ContactsContract.Contacts.CONTENT_TYPE); //Set the data type of the content in contacts, MIME type which provides directory of people
                intent.putExtra(ContactsContract.Intents.Insert.PHONE,phoneNumber); //extra field for contact phoen number, string constant used to create contact intent
                startActivity(intent);
            }
        });
    }
    public void inputNumber(View V){
        Button btn=(Button)V;
        String digit=btn.getText().toString();//5  //2
        String phoneNumber=phoneNumberEditText.getText().toString();//98  //984 //9845
        phoneNumberEditText.setText(phoneNumber +digit);//98+4  //984+5  //9845+2
    }
}

Output: 
 
 	 	 


🅴🅽🅳
🅴🅽🅳

