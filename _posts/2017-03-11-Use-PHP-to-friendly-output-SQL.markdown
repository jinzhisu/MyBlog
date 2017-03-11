---
layout: post
title:  "Hello GitHub!"
date:   2017-03-11 20:28:21
categories: program
---

If use `echo` output sql,you will see the sql is so long in the screen.

![Show SQL](http://storage.xiaoaix.cn/QQ%E6%88%AA%E5%9B%BE20170311200509.jpg)


If you hope to output sql  friendly in the screen,you can use the following function.

    /**
     * friendly output sql
     * @param String $sql 
     */
    function printf_sql($sql){
    
        $sqlTokenList = explode(' ',$sql);      // To get the phrase after split a sql by space
        $keywordList = array('SELECT','FROM','LEFT','RIGHT','INNET','WHERE','AND','GROUP','ORDER','LIMIT'); // sql keyword
        $formatSql = '';                // Declare formatted SQL
        
        // Iterate keyword
        foreach($sqlTokenList as $item => $value){
            
            if(in_array(strtoupper($value),$primaryKeyList)){
            
                // If $value belong to $parmaryKeyList ，Then newlines.And heiglight show
                $formatSql = $formatSql . '<br />' . "<span style='color:red'>" . strtoupper($value) .'</span>';
            }else{
                // To link phrase ，and forget to add blank
                $formatSql .= ' '.$value.' ';
            }
        }
        echo $formatSql;
    }

As you can see,in the function,iterte the keyword of SQL which declared before .And add `<br />` before the keyword .Final,keyword added style can highlight show.


> There is another advantage is that we can copy SQL to Command line ，then exec. 

![Copy sql to command  line](http://storage.xiaoaix.cn/QQ%E6%88%AA%E5%9B%BE20170311200956.jpg)

