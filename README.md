<!DOCTYPE HTML>
<html>

<head>
    <meta charset="utf-8">
    <title>Сфотографируйся со снеговиком</title>
    <script type="text/javascript" src="ua-parser.min.js"></script>


</head>

<body>
    <script type="text/javascript">
        document.addEventListener("DOMContentLoaded", ChooseARContent);



        function ChooseARContent() {
            var parser = new UAParser();
            var OS = parser.getOS().name;
            OS = OS.toLowerCase();
            console.log(OS);
            alert(OS);

            var elem = document.getElementById("slot");
            if (OS == "windows") {
                //elem.innerHTML = '<img src="https://github.com/eman-insilico/AR-Quick-Look-examples/raw/master/Face%20tracking%20icon.JPG" width="250" height="250">';
            } else if (OS == "android") {
                //window.location.href = "http://example.com";
            } else {
                window.location.href = "https://example.com";
            }
        }
    </script>

    <div id="slot">
        <p>
            Paragraph!
        </p>
        get your asses back here!
    </div>


</body>

</html>
