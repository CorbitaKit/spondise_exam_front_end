<template>
    <div>
        <table id="customers">
            <tr>
                <th>Name</th>
                <th>Email</th>
                <th>last login</th>
            </tr>
            <tr>
                <td>{{ user.name }}</td>
                <td>Maria Anders</td>
                <td>Germany</td>
            </tr>
            
        </table>
    </div>
</template>
<script>
    props: {
        user: Object
    }
</script>
<style>
#customers {
  font-family: Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

#customers td, #customers th {
  border: 1px solid #ddd;
  padding: 8px;
}

#customers tr:nth-child(even){background-color: #f2f2f2;}

#customers tr:hover {background-color: #ddd;}

#customers th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: left;
  background-color: #04AA6D;
  color: white;
}
</style>