<!DOCTYPE html>
<html>
    <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Image Gallery</title>
      <style>body{
    text-align: center;
}
div{
    background: url(https://wallpaper-house.com/data/out/10/wallpaper2you_403775.jpg);
    
}
p{
    background-color: white;
}
h1{
    color:white;
}</style>
    </head>
    <body>
        <div>
        <h1>
            Dev Tours and Travels 
            <hr>
            <br>
            ABOUT US
            </h1>
            <P>
                Our mission is to be the leading and most trustworthy travel management company that sets the standard for realiability and transparency to our custumers.
                </P><br><br><br><br><br><br><br><br>
        </div>
<hr>
    <img id="main-image" src="https://live-liamtra-blog.s3.ap-south-1.amazonaws.com/2021/01/Beach-Lover-3-1024x546.jpg" width="400">

    <br>
    <br>

    <img class="thumbnail" src="https://thumbs.dreamstime.com/b/breathtaking-tropical-beach-scene-swaying-palm-trees-mesmerizing-sunset-330195710.jpg" width="100">
    <img class="thumbnail" src="https://media.istockphoto.com/id/938335974/photo/aerial-view-of-kualoa-area-of-oahu-hawaii.webp?b=1&s=170667a&w=0&k=20&c=ns4dBIVWHwuLez8b3A13qA-gEeFQ8uTnWTgI4W91zcY=" width="100">
    <img class="thumbnail" src="https://static.vecteezy.com/system/resources/previews/032/951/484/large_2x/a-beautiful-beach-with-mountains-in-the-background-ai-generated-free-photo.jpg" width="100">

    <script>
        let mainImage = document.getElementById("main-image");
        let thumbnails = document.querySelectorAll(".thumbnail");

        thumbnails.forEach(img => {
            img.addEventListener("click", function() {
                mainImage.src = this.src; 
            });
        });
    </script>
    </body>
</html>
