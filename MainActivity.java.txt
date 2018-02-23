package com.example.ladoo.quizapp;

import android.content.Intent;
import android.net.Uri;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.RadioButton;
import android.widget.TextView;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }

    public void done(View view) {
        // for user input name
        EditText nameField = (EditText) findViewById(R.id.name_field);
        String name = nameField.getText().toString();


        // is the button now checked
        boolean checked = ((RadioButton) view).isChecked();
        // Check which radio button was clicked
        switch (view.getId()) {
            case R.id.radiobuttonone:
                if (checked)

                    break;
                Toast.makeText(this, "FIRST BUTTON", Toast.LENGTH_SHORT).show();
            case R.id.radiobuttontwo:
                if (checked)

                    break;
                Toast.makeText(this, "SECOND BUTTON", Toast.LENGTH_SHORT).show();


        }

    }
}





