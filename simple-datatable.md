# Simplest Data Table 

* In this code table is hardcoded but the feature of search , sorting , pagination will be provided by Datatable. Simple yet powerful.

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
	<table id="my_table">
        <thead>
			<tr role="row">
				<th>Title </th>
				<th>Name</th>
				<th>Qualification </th>
				<th>Location</th>
			</thead>
				<tr>
				<td>Doctor</td>
				<td>Mr B</td>
				<td>MBBS</td>
				<td>Mumbai</td>
			</tr>
			<tr>
				<td>Engineer</td>
				<td>Mr C</td>
				<td>PhD</td>
				<td>Delhi</td>
			</tr>
		
			<!--
			
			Copy paste set of <tr>  block atleast 10 more times to see pagination in action
			
			->
			
			<tr>
				<td>Director</td>
				<td>Mr F</td>
				<td>MBA</td>
				<td>Mumbai</td>
			</tr>
			
</table>

<script type="text/javascript">
	$(document).ready(function() {
  		 $('#my_table').DataTable();
	} );
</script>

</body>
</html>
```


## You can turn of various features like ordering or info or search etc.
[Data Table Feature Reference ] (https://datatables.net/reference/option/)
```

 $('#my_table').DataTable({
  		 
	      "paging":   true,
     	      "ordering": false,
              "info":     false,
               "searching": false,
	       "scrollY" : 300
	});

```


