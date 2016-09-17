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
<a>&nbsp;core  --------------  <a><br>
<a>&nbsp;&nbsp;&nbsp;estimate  --------------  <a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AbsoluteDiscountEstimator.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;EmpiricalEstimator.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Estimator.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;GoodTuringEstimator.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HybridEstimator.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;JelinekMercerEstimator.java<a><br>
<a>&nbsp;&nbsp;&nbsp;select  --------------  <a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Assigner.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BestEffortAssigner.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BFHeap.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BFItem.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;BruteForceAssigner.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;GreedyInsertAssigner.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;LocalSearchAssigner.java<a><br>
<a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RandomAssigner.java<a><br>
<a>&nbsp;&nbsp;&nbsp;CrowdDEC.java<a><br>
<a>&nbsp;&nbsp;&nbsp;CrowdQEC.java<a><br>
<a>&nbsp;&nbsp;&nbsp;Distribution.java<a><br>
<a>&nbsp;&nbsp;&nbsp;WorkerModel.java<a><br>
<a>&nbsp;worker  --------------  <a><br>
<a>&nbsp;&nbsp;&nbsp;AMTWorker.java<a><br>
<a>&nbsp;&nbsp;&nbsp;AMTWorkerPool.java<a><br>
<a>&nbsp;&nbsp;&nbsp;WorkerPool.java<a><br>
<a>&nbsp;util  --------------  <a><br>
<a>&nbsp;&nbsp;&nbsp;Domain.java<a><br>
<a>&nbsp;&nbsp;&nbsp;Histogram.java<a><br>
<a>&nbsp;&nbsp;&nbsp;KL.java<a><br>
<a>&nbsp;&nbsp;&nbsp;ScoredItem.java<a><br>
<a>&nbsp;util  --------------  <a><br>




