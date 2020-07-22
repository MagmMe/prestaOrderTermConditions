# prestaOrderTermConditions
Solution that allows add extra pdf files to  customer confirmation mail in Presta 1.7.6 

This is must have for every PrestaShop. 
Thanks to this rule, you can send files in .pdf to Your Customers. Files will be send in coffirmation mail. 
` if ($template == 'order_conf') {
                $message->attach(\Swift_Attachment::newInstance(file_get_contents('terms.pdf'), 'terms.pdf', 'application/pdf'));
                $message->attach(\Swift_Attachment::newInstance(file_get_contents('return_money.pdf'), 'return_money.pdf', 'application/pdf'));
            }  
						
						`
						
						
