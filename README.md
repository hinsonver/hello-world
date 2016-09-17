# CrowdDEC
<ul>
    <li> <a href ="#a1">Documentation</a>
    <li> <a href ="#a2">Building</a>
    <li> <a href ="#a3">Main code file structure</a>
    <li> <a href ="#a4">Test code file structure</a>
    <li> <a href ="#a5">Data</a>
## <a id="a1" name="a1"></a>[Documentation] ()
## <a id="a2" name="a2"></a>Building  
Use Apache Maven 3.0 to build this project
###Step 1  
    mvn clean install
###Step 2  
    mvn compile
###Step 3  
    mvn test 
##<a id="a2" name="a2"></a>Main code file structure  
<a>&nbsp;&nbsp;core  --------------  <a>  
<a>&nbsp;&nbsp;&nbsp;estimate  --------------  <a>  
<a>&nbsp;&nbsp;&nbsp;&nbsp;AbsoluteDiscountEstimator.java<a>
<a>&nbsp;&nbsp;&nbsp;&nbsp;EmpiricalEstimator.java<a>
<a>&nbsp;&nbsp;&nbsp;&nbsp;Estimator.java<a>
<a>&nbsp;&nbsp;&nbsp;&nbsp;GoodTuringEstimator.java<a>
<a>&nbsp;&nbsp;&nbsp;&nbsp;HybridEstimator.java<a>
<a>&nbsp;&nbsp;&nbsp;&nbsp;JelinekMercerEstimator.java<a>
<a>&nbsp;&nbsp;select  --------------  <a>
--  
---Assigner.java  





