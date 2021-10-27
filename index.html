<!DOCTYPE html>
<html lang="ja">
    <head>
        <meta charset="UTF-8">
        <title>食費計算アプリ（家計簿）</title>
    </head>
    <body>
        
        食費計算アプリ（家計簿）<br/>
        <form method="post">
            <input type="text" name="syokuhi">円<br/>
            <input type="hidden" name="date">
            <input type="submit" name="add" value="追加">
            <input type="submit" name="delete" value="削除">
        </form>

        <?php

        if(isset($_POST['syokuhi']) || isset($_POST['date']))
        {

        $syokuhi=$_POST['syokuhi'];

        $date=$_POST['date'];

        
        date_default_timezone_set('Asia/Tokyo');

        $date = date('Y-m-d');

        $date = $date;



            
                    if(isset($_POST['add'])==true)
                    {

                        if(preg_match('/^[0-9]+$/u',$syokuhi))
                        {
                        
                                try
                                {
                                    
                                            $syokuhi = htmlspecialchars($syokuhi,ENT_QUOTES,'UTF-8');
                                            $date = htmlspecialchars($date,ENT_QUOTES,'UTF-8');
                                    
                                            $dsn = 'mysql:dbname=syokuhi;host=localhost;charset=utf8';
                                            $user = 'root';
                                            $password = '';
                                            $dbh = new PDO($dsn, $user, $password);
                                            $dbh->setAttribute(PDO::ATTR_ERRMODE,PDO::ERRMODE_EXCEPTION);
                                            $sql = 'INSERT INTO syokuhi_log(syokuhi,date) VALUES(?,?)';
                                            $stmt = $dbh->prepare($sql);
                                            $data[] = $syokuhi;
                                            $data[] = $date;
                                            $stmt->execute($data);
                                    
                                            $dbh = null;
                                    
                                            print'食費を追加しました<br/>';
            
                                }
                                
            
                                            catch(Exception $e)
                                            {
                                                print'ただいま障害により大変ご迷惑をお掛けしております';
                                                exit();
                                            }

                                        }
                                        else
                                        {
                                            print '半角数字を記入してください<br/>';
                                        }
                        
            
            
                    } elseif(isset($_POST['delete'])==true) {
                        try
                        {
            
                            $syokuhi = htmlspecialchars($syokuhi,ENT_QUOTES,'UTF-8');
                                    
                            $dsn = 'mysql:dbname=syokuhi;host=localhost;charset=utf8';
                            $user = 'root';
                            $password = '';
                            $dbh = new PDO($dsn, $user, $password);
                            $dbh->setAttribute(PDO::ATTR_ERRMODE,PDO::ERRMODE_EXCEPTION);
                            $sql = 'DELETE FROM syokuhi_log';
                            $stmt = $dbh->prepare($sql);
                            $data[] = $syokuhi;
                            $stmt->execute($data);
                    
                            $dbh = null;
                    
                            print'食費を削除しました<br/>';

            
            
                        }
                        catch(Exception $e)
                        {
                            print'ただいま障害により大変ご迷惑をお掛けしております';
                            exit();
                        }
            
            
                    }

                        
        $dsn = 'mysql:dbname=syokuhi;host=localhost;charset=utf8';
        $user = 'root';
        $password = '';
        $dbh = new PDO($dsn, $user, $password);
        $dbh->setAttribute(PDO::ATTR_ERRMODE,PDO::ERRMODE_EXCEPTION);
        $sql = 'SELECT SUM(syokuhi) FROM syokuhi_log';
        $stmt = $dbh->prepare($sql);
        $data[] = $syokuhi;
        $stmt->execute($data);

        $dbh = null;

        $log = $stmt->fetch(PDO::FETCH_ASSOC);

        $syokuhi = $log['SUM(syokuhi)']; 
        


        print'<br/>現在の食費:';
        print $syokuhi;
        print'円';

                }

        ?>


        <?php

            $dsn = 'mysql:dbname=syokuhi;host=localhost;charset=utf8';
            $user = 'root';
            $password = '';
            $dbh = new PDO($dsn, $user, $password);
            $dbh->setAttribute(PDO::ATTR_ERRMODE,PDO::ERRMODE_EXCEPTION);
            $sql = 'SELECT * FROM syokuhi_log ORDER BY code DESC';
            $stmt = $dbh->prepare($sql);
            $stmt->execute();

            $dbh = null;




            print '<br/>';
            print '<br/>過去の食費履歴<br/>';

            while($log = $stmt->fetch(PDO::FETCH_ASSOC)) {

                
                            $syokuhi = $log['syokuhi']; 
                            $date = $log['date']; 
                
                            print $syokuhi;
                            print '円　';
                
                            print $date;
                            print'<br/>';
                
            }

            


        ?>






    </body>
</html>