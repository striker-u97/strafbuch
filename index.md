<!DOCTYPE html>
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta http-equiv="cache-control" content="no-cache" />
<meta name="viewport" content="width=device-width, initial-scale=1">
<head>
    <title>Welcome to my Lan-Play-Server</title>
    <!-- Bootstrap core CSS -->
    <link href="vendor/bootstrap/css/bootstrap.min.css" rel="stylesheet">
    <!-- Custom styles for this template -->
    <link href="css/layout.css" rel="stylesheet">
</head>
<body>
<div class="header">
    <h1><strong>Welcome to Nook-HQ Server</strong></h1>
</div>
<div class="topnav">
    <?php include "./includes/headnav.php";?>
</div>




<div class="row">
    <div class="column">
    </div>

    <div class="column table-responsive">
    <?php include './includes/indexc.php';?>
    </div>

    <!-- Bootstrap core JavaScript -->
    <script src="vendor/jquery/jquery.min.js"></script>
    <script src="vendor/bootstrap/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-sheetrock/1.1.4/dist/sheetrock.min.js"></script>
    <script>
        function copyToClipboard(element) {
            var $temp = $("<input>");
            $("body").append($temp);
            $temp.val($(element).text()).select();
            document.execCommand("copy");
            $temp.remove();
        }
    </script>
    <script>
        var mySpreadsheet = 'https://docs.google.com/spreadsheets/d/1QmgNGFPp_MFVlpImpiRIYPUI5KTR9ZkjWEnzsxMkT5g/edit#gid=1754335654';

        $("#my-table").sheetrock({
            url: mySpreadsheet
        });
    </script>
    <div class="column">
    </div>
</div>
	<div class="footer">
	<?php include './includes/footer.php';?>
	</div>
</body>
</html>


