# Export HTML table into Excel using Datatable

* Sometimes you want to export HTML table into Excel . Datatable provides you native functionality using jszip.
You can also export into pdf , csv etc. This example focuses on export html table into excel *.xsls format.

* In jquery datatable method B in lBtrip defines the button

```
<!DOCTYPE html>

<html lang="en">
<head>
  <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.10.16/css/jquery.dataTables.min.css">
  <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/buttons/1.5.1/css/buttons.dataTables.min.css">


	<script type="text/javascript" language="javascript" src="https://code.jquery.com/jquery-1.12.4.js"></script>
	
	<script type="text/javascript" language="javascript" src="https://cdn.datatables.net/1.10.16/js/jquery.dataTables.min.js"></script>
	<script type="text/javascript" language="javascript" src="https://cdn.datatables.net/buttons/1.5.1/js/dataTables.buttons.min.js"></script>
	
	<script type="text/javascript" language="javascript" src="https://cdnjs.cloudflare.com/ajax/libs/jszip/3.1.3/jszip.min.js"></script>
	<script type="text/javascript" language="javascript" src="https://cdn.datatables.net/buttons/1.5.1/js/buttons.html5.min.js"></script>

	
</head>

<body>

<h1> Table to Export in Excel </h1>

<table id="my_table" class="table table-striped table-hover display" style="width:100%">

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
			<tr>
				<td>Lawyer</td>
				<td>Mr D</td>
				<td>B.Law</td>
				<td>Nashik</td>
			</tr>
			<tr>
				<td>Doctor</td>
				<td>Mr J</td>
				<td>MBA</td>
				<td>Russia</td>
			</tr>
			<tr>
				<td>Director</td>
				<td>Mr F</td>
				<td>MBA</td>
				<td>Mumbai</td>
			</tr>
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
			<tr>
				<td>Lawyer</td>
				<td>Mr D</td>
				<td>B.Law</td>
				<td>Nashik</td>
			</tr>
			<tr>
				<td>Doctor</td>
				<td>Mr J</td>
				<td>MBA</td>
				<td>Russia</td>
			</tr>
			<tr>
				<td>Director</td>
				<td>Mr F</td>
				<td>MBA</td>
				<td>Mumbai</td>
			</tr>
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
			<tr>
				<td>Lawyer</td>
				<td>Mr D</td>
				<td>B.Law</td>
				<td>Nashik</td>
			</tr>
			<tr>
				<td>Doctor</td>
				<td>Mr J</td>
				<td>MBA</td>
				<td>Russia</td>
			</tr>
			<tr>
				<td>Director</td>
				<td>Mr F</td>
				<td>MBA</td>
				<td>Mumbai</td>
			</tr>
			
</table>



<script type="text/javascript">
	$(document).ready(function() {
  		 $('#my_table').DataTable( {
        "dom": "lBtrip",
        buttons: [{
        		text: 'Export This Table To Excel',                       
                extend: 'excelHtml5'}]
    } );
	} );
</script>
</body>
</html>

```
