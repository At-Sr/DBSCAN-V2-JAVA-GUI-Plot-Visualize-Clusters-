# DBSCAN-V2-JAVA-GUI-Plot-Visualize-Clusters-
DBSCAN V2+ JAVA GUI (Plot/Visualize Clusters)
PSEUDOCODE
-------------------------------------

DBSCAN(D, eps, MinPts)
   C = 0
   for each unvisited point P in dataset D
      mark P as visited
      N = getNeighbors (P, eps)
      if sizeof(N) < MinPts
         mark P as NOISE
      else
         C = next cluster
         expandCluster(P, N, C, eps, MinPts)
          
expandCluster(P, N, C, eps, MinPts)
   add P to cluster C
   for each point P' in N 
      if P' is not visited
         mark P' as visited
         N' = getNeighbors(P', eps)
         if sizeof(N') >= MinPts
            N = N joined with N'
      if P' is not yet member of any cluster
         add P' to cluster C
		 
---------------------------------------
![Capture 00](https://github.com/AthmaneSrai/DBSCAN-V2-JAVA-GUI-Plot-Visualize-Clusters-/tree/master/Screenshots/Capture%00.PNG)
![Capture 01](https://github.com/AthmaneSrai/DBSCAN-V2-JAVA-GUI-Plot-Visualize-Clusters-/tree/master/Screenshots/Capture 01.PNG)
![Capture 2](https://github.com/AthmaneSrai/DBSCAN-V2-JAVA-GUI-Plot-Visualize-Clusters-/tree/master/Screenshots/Capture 2.PNG)
![Capture 3](https://github.com/AthmaneSrai/DBSCAN-V2-JAVA-GUI-Plot-Visualize-Clusters-/tree/master/Screenshots/Capture 3.PNG)
![Capture 4](https://github.com/AthmaneSrai/DBSCAN-V2-JAVA-GUI-Plot-Visualize-Clusters-/tree/master/Screenshots/Capture 4.PNG)
![Capture 5](https://github.com/AthmaneSrai/DBSCAN-V2-JAVA-GUI-Plot-Visualize-Clusters-/tree/master/Screenshots/Capture 5.PNG)
![Capture 6](https://github.com/AthmaneSrai/DBSCAN-V2-JAVA-GUI-Plot-Visualize-Clusters-/tree/master/Screenshots/Capture 6.PNG)
![Capture 7](https://github.com/AthmaneSrai/DBSCAN-V2-JAVA-GUI-Plot-Visualize-Clusters-/tree/master/Screenshots/Capture 7.PNG)



