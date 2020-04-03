@Author- RAM
1- Get all Employee 
Get: http://localhost:8081/api/employee
[
  {
    "ENAME": "SMITH",
    "COMM": null,
    "MGR": 7902,
    "EMPNO": 7369,
    "JOB": "CLERK",
    "HIREDATE": "2020-03-24T00:00:00",
    "DEPTNO": 20,
    "SAL": 800
  },
  {
    "ENAME": "ALLEN",
    "COMM": 300,
    "MGR": 7698,
    "EMPNO": 7499,
    "JOB": "SALESMAN",
    "HIREDATE": "2020-03-24T00:00:00",
    "DEPTNO": 30,
    "SAL": 1600
  },
  {
    "ENAME": "WARD",
    "COMM": 500,
    "MGR": 7698,
    "EMPNO": 7521,
    "JOB": "SALESMAN",
    "HIREDATE": "2020-03-24T00:00:00",
    "DEPTNO": 30,
    "SAL": 1250
  },
  {
    "ENAME": "JONES",
    "COMM": null,
    "MGR": 7839,
    "EMPNO": 7566,
    "JOB": "MANAGER",
    "HIREDATE": "2020-03-24T00:00:00",
    "DEPTNO": 20,
    "SAL": 2975
  },
  {
    "ENAME": "MILLER",
    "COMM": null,
    "MGR": 7782,
    "EMPNO": 7934,
    "JOB": "CLERK",
    "HIREDATE": "2020-03-24T00:00:00",
    "DEPTNO": 10,
    "SAL": 1300
  }
]

2-Get Employe by empno

Get: http://localhost:8081/api/employee?empno=7369 
[
  {
    "ENAME": "SMITH",
    "COMM": null,
    "MGR": 7902,
    "EMPNO": 7369,
    "JOB": "CLERK",
    "HIREDATE": "2020-03-24T00:00:00",
    "DEPTNO": 20,
    "SAL": 800
  }
]

-Create Employee Data-
POST: http://localhost:8081/api/employee

Json request
{
	
"EMPNO":"63534",
"ENAME":"AMIT JAIN",
"JOB":"SALES",
"MGR":"7698",
"HIREDATE":"2020-03-24",
"SAL":"12536",
"COMM":"23"
}
Json Response message - "Data Save Successfully !!!"

-UPDATE Employee Data-
POST: http://localhost:8081/api/employee?empno=63534

{
"ENAME":"AMIT JAIN",
"JOB":"SALES",
"MGR":"7698",
"HIREDATE":"2020-03-24",
"SAL":"7863",
"COMM":"22"
}
Json Response message - "Data Updated Successfully !!!"


-Delete Employee data via EMPNO

DELETE: http://localhost:8081/api/employee?empno=63534
Json Response message - "Data has been deleted successfully !!!"
