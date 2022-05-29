# paginationforvue
custom pagination for vue.js
place the container file in the container folder 
then use the file via 
in vue file you want to use 

In <script> part write those code 
import the file 
import Pagination from '@/containers/Pagination';
use it in components
components: { Pagination },
And
add this on method
 loadData: function (offset = 0) 
{
  
 }
  
AND
In <template> part copy this code 
<pagination :paginationData=total_rows @pagination="loadData"></pagination>
  
there you need to pass to vaule  
total_rows is number of total data of that table
And
loadData is name of the function that call api to   
