# prestaOrderTermConditions

Solution that allows add extra pdf files to  customer confirmation mail in Presta 1.7.6 or higher

This is must have for every PrestaShop. 
Thanks to this rule, you can send files in .pdf to Your Customers. Files will be send in coffirmation mail. 			

`if ($template == 'order_conf') {
                $message->attach(\Swift_Attachment::newInstance(file_get_contents('regulamin.pdf'), 'regulamin.pdf', 'application/pdf'));
                $message->attach(\Swift_Attachment::newInstance(file_get_contents('formularz_zwrotu.pdf'), 'formularz_zwrotu.pdf', 'application/pdf'));
            }`					
						
						
How to add this line of code?
1. Go to -> classes (main directory) -> mail.php
2. Find line no. 566.
3. Below this line just paste this code.
4. Change names of Your files and do not forget to add these files to your presta. 

If You want, You can dowload ready file from this repo. 

Enjoy!


