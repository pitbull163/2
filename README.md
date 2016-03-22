# 2
         
              equire_once("QIWIControl.php")


construct

-require_once("QIWIControl.php");
-$qiwi = new QIWIControl("+79277706967", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
-if(!$qiwi->login()){
-    if($err = $qiwi->getLastError()){
-        die("Failed to login into QIWI Wallet: " . $err['message'])

    require_once("QIWIControl.php");
    $qiwi = new QIWIControl("+79277706967", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
    if(!$qiwi->login()){
        if($err = $qiwi->getLastError()){
           die("Failed to login into QIWI Wallet: " . $err['message'])
       } 
        die("Failed to login into QIWI wallet.")
}
-    die("Failed to login into QIWI wallet.");
-}
-$qiwi->newOrder("+7968045422", 1500, "RUB", "Счет №22112210")


-require_once("QIWIControl.php");
-$qiwi = new QIWIControl("+79681234433", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
-if(!$qiwi->login()){
-    if($err = $qiwi->getLastError()){
-        die("Failed to login into QIWI Wallet: " . $err['message'])

, +    require_once("QIWIControl.php");
+    $qiwi = new QIWIControl("+79681234433", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
+    if(!$qiwi->login()){
+        if($err = $qiwi->getLastError()){
+            die("Failed to login into QIWI Wallet: " . $err['message']);
+        }
+        die("Failed to login into QIWI wallet.");
     }
-    die("Failed to login into QIWI wallet.");
-}
-$tr = $qiwi->loadBills(QIWI_BILLS_MODE_INOUT, "15.12.2015", "16.12.2015");
-print_r($tr);
+    $tr = $qiwi->loadHistoryDateRange("18.10.2015", "06.11.2015");
+    print_r($tr)

Array
+(
+    [0] => Array
+        (
+            [id] => 2071000178869449 
+            [status] => 1
+            [statusText] => Success
+            [date] => 06.11.2015
+            [time] => 20:54:00
+            [datetime] => 06.11.2015 20:54:00
+            [provider] => Покупка TK KNAKER IVAKINO, карта 4693****2209
+            [comment] => TK KNAKER IVAKINO>KHIMKI MEZHDU       RU
+            [cash] => -188
+        )
+
+    [1] => Array
+        (
+            [id] => 2071000178708383 
+            [status] => 1
+            [statusText] => Success
+            [date] => 06.11.2015
+            [time] => 12:51:56
+            [datetime] => 06.11.2015 12:51:56
+            [provider] => Покупка TK KNAKER IVAKINO, карта 4693****2209
+            [comment] => TK KNAKER IVAKINO>KHIMKI MEZHDU       RU
+            [cash] => -194
+        )
+
+    [2] => Array
+        (
+            [id] => 2071000178511602 
+            [status] => 1
+            [statusText] => Success
+            [date] => 05.11.2015
+            [time] => 15:44:56
+            [datetime] => 05.11.2015 15:44:56
+            [provider] => Покупка TK KNAKER IVAKINO, карта 4693****2209
+            [comment] => TK KNAKER IVAKINO>KHIMKI MEZHDU       RU
+            [cash] => -575
+        )
 
+    [3] => Array
+        (
+            [id] => 1121100737337608 
+            [status] => 1
+            [statusText] => Success
+            [date] => 05.11.2015
+            [time] => 10:42:23
+            [datetime] => 05.11.2015 10:42:23
+            [provider] => Visa QIWI Wallet QIWI Bank
+            [comment] => Пополнение или возврат платежа по QVC\QVP
+            [cash] => 3553
+        )
+)
+loadHistoryToday
  loadHistoryDateRange
+loadHistoryYesterday
 
 loadHistoryDateRange
+loadHistoryLastWeek
 
-Array ( 

[0] => Array ( [id] => 6787569830 [status] => 4 [statusText] => Canceled [payDate] => 15.01.2016 [from] => [to] => 79680675327 [creationDate] => 16.12.2015 [comment] => Привет! [cash] => 15 ) 
[1] => Array ( [id] => 6787517188 [status] => 4 [statusText] => Canceled [payDate] => 15.01.2016 [from] => [to] => 79680675327 [creationDate] => 16.12.2015 [comment] => [cash] => 11 ) 
[2] => Array ( [id] => 6787335314 [status] => 4 [statusText] => Canceled [payDate] => 15.01.2016 [from] => [to] => 71221123123 [creationDate] => 16.12.2015 [comment] => comment [cash] => 11 )
[3] => Array ( [id] => 6787099352 [status] => 4 [statusText] => Canceled [payDate] => 15.01.2016 [from] => Visa QIWI Wallet 79841545864 [to] => [creationDate] => 16.12.2015 [comment] => [cash] => 1 )
[4] => Array ( [id] => 6786681911 [status] => 1 [statusText] => Paid [payDate] => 15.01.2016 [from] => [to] => 79841545864 [creationDate] => 16.12.2015 [comment] => Счет №2211334455 [cash] => 1 ) 
[5] => Array ( [id] => 6784361288 [status] => 4 [statusText] => Canceled [payDate] => 14.01.2016 [from] => [to] => 79680675327 [creationDate] => 15.12.2015 [comment] => Проверка  [cash] => 1 ) 
)
 loadHistoryDateRange
+findTransaction
-require_once("QIWIControl.php");
-$qiwi = new QIWIControl("+79681234433", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
-if(!$qiwi->login()){
-    if($err = $qiwi->getLastError()){
-        die("Failed to login into QIWI Wallet: " . $err['message'])


+    require_once("QIWIControl.php");
+    $qiwi = new QIWIControl("+79681234433", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
+    if(!$qiwi->login()){
+        if($err = $qiwi->getLastError()){
+            die("Failed to login into QIWI Wallet: " . $err['message']);
+        }
+        die("Failed to login into QIWI wallet.");
     }
-    die("Failed to login into QIWI wallet.");
-}
-$tr = $qiwi->loadHistoryDateRange("18.10.2015", "06.11.2015");
-$tr = $qiwi->findTransaction($tr, -596, "APTEKA");
-print_r($tr);
+    $tr = $qiwi->loadHistoryDateRange("18.10.2015", "06.11.2015");
+    $tr = $qiwi->findTransaction($tr, -596, "APTEKA");
+    print_r($tr);

+    require_once("QIWIControl.php");
+    $qiwi = new QIWIControl("+79681234433", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
+    if(!$qiwi->login()){
+        if($err = $qiwi->getLastError()){
+            die("Failed to login into QIWI Wallet: " . $err['message']);
+        }
+        die("Failed to login into QIWI wallet.");
+    }
+    $qiwi->newOrder("+7968045422", 1500, "RUB", "Счет №22112210");
+
+Функция возвращает или true в случае успеха или false в случае ошибки.
+loadBills
+Array
+(
+    [0] => Array
+        (
+            [id] => 2071000176482982 
+            [status] => 1
+            [statusText] => Success
+            [date] => 26.10.2015
+            [time] => 19:44:52
+            [datetime] => 26.10.2015 19:44:52
+            [provider] => Покупка APTEKA FORTE, карта 4693****2209
+            [comment] => APTEKA FORTE>KHIMKI                   RU
+            [cash] => -596
+        )
+
+)
+findTransactionByAmount
+
+Функция позволяет получать список счетов как выставленных на текущий кошелек (входящие счета), так и выставленных с текущего кошелька (исходящие счета). Структура счетов схожа со структурой транзакций. Если параметры $dateFrom и $dat или false в случае ошибк
+
+    $mode — Режим работы со счетами. Если хотим получить и входящие и исходящие счета, то мы должны указать здесь значение QIWI_BILLS_MODE_INOUT, если хотим получить только входящие QIWI_BILLS_MODE_IN, исходящие QIWI_BILLS_MODE_OUT.
+    $dateFrom — Дата начала поиска счетов. Будут загружены счета, созданные начиная с этой даты. Можно не указывать, если указан параметр $dateTo.
+    $date
      $dateFrom.


+    require_once("QIWIControl.php");
+    $qiwi = new QIWIControl("+79681234433", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
+    if(!$qiwi->login()){
+        if($err = $qiwi->getLastError()){
+            die("Failed to login into QIWI Wallet: " . $err['message']);
+        }
+        die("Failed to login into QIWI wallet.");
+    }
+    $tr = $qiwi->loadBills(QIWI_BILLS_MODE_INOUT, "15.12.2015", "16.12.2015");
+    print_r($tr)

+Array
+(
+    [0] => Array
+        (
+            [id] => 6787569830
+            [status] => 4
+            [statusText] => Canceled
+            [payDate] => 15.01.2016
+            [from] => 
+            [to] => 79680675327
+            [creationDate] => 16.12.2015
+            [comment] => Привет!
+            [cash] => 15
+        )
+
+    [1] => Array
+        (
+            [id] => 6787517188
+            [status] => 4
+            [statusText] => Canceled
+            [payDate] => 15.01.2016
+            [from] => 
+            [to] => 79680675327
+            [creationDate] => 16.12.2015
+            [comment] => 
+            [cash] => 11
+        )
+
+    [2] => Array
+        (
+            [id] => 6787335314
+            [status] => 4
+            [statusText] => Canceled
+            [payDate] => 15.01.2016
+            [from] => 
+            [to] => 71221123123
+            [creationDate] => 16.12.2015
+            [comment] => comment
+            [cash] => 11
+        )
+
+    [3] => Array
+        (
+            [id] => 6787099352
+            [status] => 4
+            [statusText] => Canceled
+            [payDate] => 15.01.2016
+            [from] => Visa QIWI Wallet 79841545864
+            [to] => 
+            [creationDate] => 16.12.2015
+            [comment] => 
+            [cash] => 1
+        )
+
+    [4] => Array
+        (
+            [id] => 6786681911
+            [status] => 1
+            [statusText] => Paid
+            [payDate] => 15.01.2016
+            [from] => 
+            [to] => 79841545864
+            [creationDate] => 16.12.2015
+            [comment] => Счет №2211334455
+            [cash] => 1
+        )
+
+    [5] => Array
+        (
+            [id] => 6784361288
+            [status] => 4
+            [statusText] => Canceled
+            [payDate] => 14.01.2016
+            [from] => 
+            [to] => 79680675327
+            [creationDate] => 15.12.2015
+            [comment] => Проверка выставления счета
+            [cash] => 1
+        )
+loadBalance

+    require_once("QIWIControl.php");
+    $qiwi = new QIWIControl("+79681234433", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
+    if(!$qiwi->login()){
+        if($err = $qiwi->getLastError()){
+            die("Failed to login into QIWI Wallet: " . $err['message']);
+        }
+        die("Failed to login into QIWI wallet.");
+    }
+    if(($balance = $qiwi->loadBalance()) !== false){
+        echo "BALANCE RUB={$balance['RUB']}\n";
+        echo "BALANCE EUR={$balance['EUR']}\n";
+        echo "BALANCE USD={$balance['USD']}\n";
+    }else{
+        die("Failed to get QIWI balance.\n");
+    }
+BALANCE RUB=11933.21
+BALANCE EUR=0
+BALANCE USD=0
+transferMoney
+    require_once("QIWIControl.php");
+    $qiwi = new QIWIControl("+79681234433", "myPwd1", "cookie_data", "payproxys.ru:3128", "account1:accPWD2211", true);
+    if(!$qiwi->login()){
+        if($err = $qiwi->getLastError()){
+            die("Failed to login into QIWI Wallet: " . $err['message']);
+        }
+        die("Failed to login into QIWI wallet.");
+    }
+    if(!($trInfo = $qiwi->transferMoney("+79680671122", "RUB", 1015.12, "Просто перевод"))){
+        die("Failed to transfer money to another QIWI wallet.");
+    }
+    echo "Transaction info:";
+    print_r($trInfo);
+Array
+(
+    [id] => 7100329842
+    [state] => Array
+        (
+            [code] => AwaitingSMSConfirmation
+        )
+
+    [paymentId] => 1455195743806
+)
+
+cofirmSMSCode

