# How to output PHP array as a table
Output array as table

```
echo '<table border="1">';
echo '<tr>';
foreach ($rows_data[0] as $key => $value) {
    echo '<td>'.$key.'</td>';
}
echo '</tr>';


foreach ($rows_data as $key => $values) {
  echo '<tr>';
  foreach ($values as $key2 => $value) {

   //if ($key2=='datatime') {$value = date('d.n.y',$value); } //If you need to process some columns, for example timestamp
   echo '<td>'.$value.'</td>';
 }
 echo '</tr>';
}

echo '</table>';
```
