<!DOCTYPE html>
<html >
<head>
 <title>Student Details with CGPA</title>
 <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.2/angular.min.js"> 
</script>
</head>
<body ng-app="myApp">
<div ng-controller="myController">
 <h2>Student Details</h2>
 <p>Total number of students: {{ students.length }}</p>
 <table border="1">
 <tr>
 <th>Name</th>
 <th>CGPA</th>
 </tr>
 <tr ng-repeat="student in students">
 <td>{{ student.name }}</td>
 <td>{{ student.cgpa }}</td>
 </tr>
 </table>
</div>
<script src="Program5.js"> </script> 
</body>
</html>
Program5.js
var app = angular.module('myApp', []);
app.controller('myController', function ($scope) {
 // Default student details
 $scope.students = [
 { name: 'Akshaya', cgpa: 8.8 },
 { name: 'Krishna Patel', cgpa: 7.2 },
 { name: 'Johnson', cgpa: 6.5 },
 { name: 'Safwan', cgpa: 7.5},
 { name: 'Zeenath', cgpa: 8.5}
 ];
 });
