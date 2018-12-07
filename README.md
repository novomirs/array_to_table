# array_to_table
Output array as table

echo '<table border="1">';
echo '<tr>';
foreach ($rows_data[0] as $key => $value) {
    echo '<td>'.$key.'</td>';
}
echo '</tr>';


foreach ($rows_data as $key => $values) {
  echo '<tr>';
  foreach ($values as $value) {

   //if ($key=='datatime') {$value = date('d.n.y',$value); }
   echo '<td>'.$value.'</td>';
 }
 echo '</tr>';
}


echo '</table>’;
