SQL Assignment : -

https://sqliteonline.com/#sqltext=%23tab-name%3Dchinook.db%0D%0ASELECT%20c.first_name%20%7C%7C%20'%20'%20%7C%7C%20c.last_name%20AS%20CustomerName%2CSUM(i.total)%20AS%20TotalSpent%20FROM%20customer%20c%20JOIN%20invoice%20i%20%0AON%20c.customer_id%20%3D%20i.customer_id%20GROUP%20BY%20c.customer_id%20ORDER%20BY%20TotalSpent%20DESC%20LIMIT%205%3B%0A%0ASELECT%20g.name%20AS%20Genre%2CSUM(il.quantity)%20AS%20TotalTracksSold%20FROM%20invoice_line%20il%20JOIN%20track%20t%20ON%20il.track_id%20%3D%20t.track_id%0AJOIN%20genre%20g%20ON%20t.genre_id%20%3D%20g.genre_id%20GROUP%20BY%20g.genre_id%20ORDER%20BY%20TotalTracksSold%20DESC%20LIMIT%201%3B%0A%0ASELECT%20m.first_name%20%7C%7C%20'%20'%20%7C%7C%20m.last_name%20AS%20Manager%2Ce.first_name%20%7C%7C%20'%20'%20%7C%7C%20e.last_name%20AS%20Subordinate%20FROM%20employee%20e%0AJOIN%20employee%20m%20ON%20e.reports_to%20%3D%20m.employee_id%20ORDER%20BY%20Manager%3B%0A%0ASELECT%20a.name%20AS%20Artist%2Cal.Title%20AS%20Album%2CSUM(ii.quantity)%20AS%20TotalSold%20FROM%20invoice_line%20ii%0AJOIN%20track%20t%20ON%20ii.track_id%20%3D%20t.track_id%20JOIN%20album%20al%20ON%20t.album_id%20%3D%20al.album_id%0AJOIN%20artist%20a%20ON%20al.artist_id%20%3D%20a.artist_id%20GROUP%20BY%20a.artist_id%2C%20al.album_id%20%0AHAVING%20SUM(ii.Quantity)%20%3D%20(SELECT%20MAX(album_total.TotalSold)FROM%20(SELECT%20SUM(ii2.quantity)%20AS%20TotalSold%20FROM%20%0Ainvoice_line%20ii2%20JOIN%20track%20t2%20ON%20ii2.track_id%20%3D%20t2.track_id%20JOIN%20album%20al2%20ON%20t2.album_id%20%3D%20al2.album_id%0AWHERE%20al2.artist_id%20%3D%20a.artist_id%20GROUP%20BY%20al2.album_id)%20AS%20album_total)%20ORDER%20BY%20Artist%3B%0A%0ASELECT%20strftime('%25Y-%25m'%2C%20invoice_date)%20AS%20Month%2CSUM(total)%20AS%20Revenue%20FROM%20invoice%20WHERE%20strftime('%25Y'%2C%20invoice_date)%20%3D%20'2013'%0AGROUP%20BY%20Month%20ORDER%20BY%20Month%3B%0A


Tableau Assignment :-

https://public.tableau.com/views/Task-3TA/AirbnbNYC2019NeighborhoodsPricesandAvailability?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link


Excel Assignment :- 

https://docs.google.com/spreadsheets/d/1ycu9aSwMz1-ydm5KvQ26kCwcaemFIv8v/edit?usp=sharing&ouid=108116458430976589441&rtpof=true&sd=true


ChatGPT prompts :-

https://chatgpt.com/share/67f934ba-8ae0-8004-af4a-7537891e0ca3
