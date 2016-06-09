# Picasso
Picasso is an image library for Android


Download the JAR file 

It's very useful for managing images and no worry about Memory problem.
When I' download images from server or json 


Open the layout file and add an ImageView to the layout

      <ImageView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/img_product"
        android:layout_alignParentTop="true"
        android:layout_centerHorizontal="true" />
        
import statement at the top of the Activity class.

    import com.squareup.picasso.Picasso;

**in Adapter class**

        img = (ImageView) convertView.findViewById(R.id.img_product);
        String url = "https://www."+ fe.getImage_one().toString();
        url = url.replaceAll(" ", "%20");
        Picasso.with(context).load(url)
                .into(img);


You make sure to add  your project's manifest.

               <uses-permission android:name="android.permission.INTERNET" /> 
               
