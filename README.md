# DBA-lab2
1)

- check where is the location of archivelog
![Screenshot (943)](https://user-images.githubusercontent.com/93229250/231610858-a80a37e6-0607-44e0-a1d3-65886f3a6f64.png)

- switch online redo log file by command
![Screenshot (944)](https://user-images.githubusercontent.com/93229250/231610972-3835dea5-e78a-4d91-bece-6d8a13462fad.png)

- select group , archived, status from v$log ;
![Screenshot (946)](https://user-images.githubusercontent.com/93229250/231611134-561d8dc2-a513-413a-8bc7-d28c0e91343c.png)

- view the redo log files names, size, group number, status, archived or not and their sizes in MB using the views "v$log" and "v$logfile".
![Screenshot (952)](https://user-images.githubusercontent.com/93229250/231612764-70b67d55-3653-4139-ad8c-d0421af26ca4.png)
![Screenshot (948)](https://user-images.githubusercontent.com/93229250/231612374-a6fd88da-9e00-4dba-81be-f7c451b1ad66.png)

- Increase the size of all redo log files to be 100 MB, then repeat the last step.
![Screenshot (971)](https://user-images.githubusercontent.com/93229250/231619461-af03dd92-83e4-47b2-b135-dabe221b14a7.png)
![Screenshot (972)](https://user-images.githubusercontent.com/93229250/231619584-89bb6853-3bd2-4ef6-a3fd-607ac330fd92.png)


- create new three redo log file groups 4,5 and 6 then again view the redo log files names, size, group number, status, archived or not and their sizes in MB using the views "v$log" and "v$logfile"
![Screenshot (961)](https://user-images.githubusercontent.com/93229250/231617541-5941ffd0-3c7d-4b8f-8992-e50dce4857ec.png)
![Screenshot (969)](https://user-images.githubusercontent.com/93229250/231619260-f369deac-e6dc-43d5-ac35-086d7b459348.png)
![Screenshot (967)](https://user-images.githubusercontent.com/93229250/231619283-781961ca-9c24-4271-840e-b5e5ebe3a162.png)
![Screenshot (968)](https://user-images.githubusercontent.com/93229250/231619302-ad6bf3e9-0d6a-4a00-9403-b257209333bb.png)


- drop redo log group 6 ; 
![Screenshot (974)](https://user-images.githubusercontent.com/93229250/231620030-ec88cc40-aebb-4b8e-95b0-7a5b69af857b.png)


2)

- create new undo tablespace , with one datafile 50MB
![Screenshot (976)](https://user-images.githubusercontent.com/93229250/231620320-15309f84-3d1d-43f4-b3a0-270fc462a2cd.png)

- Show the value of parameter undo_retention then change the value of it to be 3 minutes and gurantee this duration.
![Screenshot (979)](https://user-images.githubusercontent.com/93229250/231621712-c25ab4be-c37a-4abb-abba-b126135500cc.png)
![Screenshot (1031)](https://user-images.githubusercontent.com/93229250/231913417-ab00bab1-6b3e-4f78-86b1-f06439a70282.png)

- make this new created tablespace the default tablespace
![Screenshot (983)](https://user-images.githubusercontent.com/93229250/231628232-a3696a9e-fd64-44bf-b939-84fb424679d3.png)

- create new tablespace ITI with one datafile with size 50MB and make it the default tablespace for HR user
- ![Screenshot (985)](https://user-images.githubusercontent.com/93229250/231631265-9d93fe7f-4b07-48b3-b62e-74841d57eef7.png)

- create temporary tablespace TEMP2 with size 50MB
![Screenshot (987)](https://user-images.githubusercontent.com/93229250/231632644-bce713ca-9013-4a4a-ab93-7ec6b7096b86.png)

- resize up the datafile of ITI tablespace from 50MB to 100MB
![Screenshot (988)](https://user-images.githubusercontent.com/93229250/231914345-f8940a55-c7ed-4080-a178-7fdcab4b2f74.png)

- show data files names, thier tablespaces, their size, their status using view "dba_data_files".
![Screenshot (989)](https://user-images.githubusercontent.com/93229250/231632689-d4c6ea9d-0ec8-4855-bc74-3b303f401249.png)



3)

- create an OS user with name "iti" and make him login to the database using "sqlplus /"
![Screenshot (993)](https://user-images.githubusercontent.com/93229250/231642899-459f0969-ea94-43c3-909b-5258a23a4973.png)

- make your personal Operating system user to connect locally with authentication as sysdba.
![Screenshot (997)](https://user-images.githubusercontent.com/93229250/231654691-0040e02d-1c64-41d6-be96-bcf105bd8a1f.png)
![Screenshot (995)](https://user-images.githubusercontent.com/93229250/231654570-4fda8cbb-a85d-4835-b717-7aaac22fbf5e.png)
![Screenshot (1033)](https://user-images.githubusercontent.com/93229250/231938565-f3aa4162-4c0d-4655-8284-7456581e5b21.png)

