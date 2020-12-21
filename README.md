package com.example.android.practiceset2;



import android.app.Activity;
import android.os.Bundle;
import android.view.View;
import android.widget.TextView;
import org.w3c.dom.Text;

/**

 This app displays an order form to order coffee.
 */
public class MainActivity extends Activity {



    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        String lastname="Fujiwara";
        String firstname="Lyla";
        String contactinfo=firstname + " " + lastname;
        contactinfo=contactinfo + " <" + lastname + "." + firstname + "@justjava.com>";
        display1(contactinfo);

    }

    public void display1(String i){
        TextView box1=(TextView) findViewById(R.id.display_text_view);
        box1.setText(""+i);

    }



}
