<p>Hello My name is Aditya Pratap Singh Chauhan, I am a student of jiit and I tried implenting gofr into my room booking website that was built for my 3rd sem DSW(Database Systems and Webtheory) lab.
I was not able to implement the same in this version of the repo but i have included the website project (in the folder "dsw") and all the progess that i have made at the backend side using gofr. 
However I was able to create and access the db "the_monarch" and the table "details" using xampp and the gofr framework...all the progress done in the gofr side of things has been saved in the folder named "gofr".</p>

<p>The following commands were ran on the admin cmd prompt</p>

```docker run --name zops-gofr-mysql -e MYSQL_ROOT_PASSWORD=root123 -e MYSQL_DATABASE=the_monarch -p 3306:3306 -d mysql:8.0.30```


```docker exec -it zops-gofr-mysql mysql -uroot -proot123 the_monarch -e "CREATE TABLE details ( name VARCHAR(255) NOT NULL PRIMARY KEY,Number int, CheckInDate date, CheckOutDate date, NoOfRooms int);"```

<p>To view the progressI have made, simply run the file gofr/hotel/another.go and go to the following urls:</p>
<ol>
<li>http://localhost:8080/</li>
<li>http://localhost:8080/details</li>
</ol>
<p>If you want to view the working of the website copy the dsw folder to htdocs of xampp and run it locally </p>

<p>All the progess is in gofr/hotel/another.go 
the framework has not been linked with the main website which is present in the dsw folder</p>
