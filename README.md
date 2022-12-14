# Git-JMO.github.io

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SIO UGS Dashboard</title>
    <link
      rel="stylesheet"
      href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
      integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm"
      crossorigin="anonymous"/>
      <link rel="stylesheet" href="static/css/style.css">
</head>
<body class="bg-dark">
    <div class="wrapper">
        <nav class="navbar navbar-dark bg-dark navbar-expand-lg">
            <a class="navbar-brand" href="index.html">UGS Data Tracker</a>
        </nav>
        <div class="jumbotron">
            <h1 class="display-4"> <b>Track Your UGS</b></h1>
        </div>
        <div class="container-fluid">
            <div class="row">
                <div class="col-md-4">
                    <h3>Do you know where your UGS are? <br><small>Look No Further!</small></h3>
                </div>
                <div class="col-md-8">
                    <p>
                        This webpage displays the latest data for your emplaced UGS. Feel free to filter by UG ID or Date.
                        <br>
                        If you have any issues with the latest data please let us know. Contact as at 
                        <br>
                        TSVOIP: 918-5904 or SVOIP: 302-458-039 and we will be happy to help.
                        <br>
                        <h2>By the way....Where is your CONOP?</h2>
                        <br><br>
                    </p>
                </div>
            </div>
        </div>
        <div class="container-fluid">
            <div class="row">
                <div class="col-md-3">
                    <form class="bg-dark">
                        <p>Filter Search</p>
                        <ul class="list-group bg-dark">
                            <li class="list-group-item bg-dark">
                                <label for="Target.Detection.detecttime">Enter Date Time Using Below Format</label>
                                <input type="text" class="form-control" placeholder="0/00/0000 0:00" id="Target.Detection.detecttime" />
                            </li>
                            <li class="list-group-item bg-dark">
                                <label for="Target.Identification.number">Enter UG ID</label>
                                <input type="text" class="form-control" placeholder="12345" id="Target.Identification.number" />
                            </li>
                            <li class="list-group-item bg-dark">
                                <label for="Target.Detection.classification">Enter Detect Type</label>
                                <input type="text" class="form-control" placeholder="Tamper" id="Target.Detection.classification" />
                            </li>
                        </ul>
                    </form>
                </div>
                <div class="col-md-9">
                    <table class="table table-striped">
                        <thead>
                            <tr>
                                <th>Target.Location.lat</th>
                                <th>Target.Location.lon	</th>
                                <th>Target.Identification.number</th>
                                <th>Target.Identification.description</th>
                                <th>Target.Detection.detecttime</th>
                                <th>Target.Detection.classification</th>
                            </tr>
                        </thead>
                        <tbody>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/d3/4.11.0/d3.js"></script>
    <script src="static/js/data.js"></script>
    <script src="static/js/app.js"></script>
</body>
</html>
