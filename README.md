# Picasso
Picasso is an image library for Android

It's very useful for managing images and no worry about Memory problem.
When I' download images from server or json 

**in Adapter class**

        img = (ImageView) convertView.findViewById(R.id.img_product);
        String url = "https://www."+ fe.getImage_one().toString();
        url = url.replaceAll(" ", "%20");
        Picasso.with(context).load(url)
                .into(img);
