# Datatable with JSON response
* I am using ( https://jsonplaceholder.typicode.com/posts ) for sample JSON . _Thanks For Making this JSON Place Holder_
* Just define the table headers and column in Data Table Requests.

```

<!DOCTYPE html>

<html lang="en">
<head>
  <link rel="stylesheet" href="./index_files/bootstrap.min.css">
  <script src="./index_files/jquery.min.js"></script>
  <link rel="stylesheet" type="text/css" href="./index_files/datatables.min.css">
  <script type="text/javascript" src="./index_files/datatables.min.js"></script>
</head>

<body>
	<table id="json_table">
	
		 <thead>
            <tr>
                <th>User Id</th>
                <th>Id</th>
                <th>Title</th>
                <th>Body</th>
            </tr>
        </thead>
	</table>
  
  
	<script type="text/javascript">
		$(document).ready(function() {
		
    $('#json_table').DataTable( {
        "ajax": {
           			 "url": "https://jsonplaceholder.typicode.com/posts",
           			 "dataSrc": ""
        		},
      
        "columns": [
          			  { "data": "userId" },
         		      { "data": "id" },
        		      { "data": "title" },
                      { "data": "body" }
         		  ]
  			  } );
		} );
	</script>

</body>
</html>


```
