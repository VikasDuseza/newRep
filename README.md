# newRep

  //Find the Search text box UI Element
            IWebElement FirstName = driver.FindElement(By.Name("FirstName"));
            IWebElement LastName = driver.FindElement(By.Name("LastName"));
            IWebElement GmailAddress = driver.FindElement(By.Name("GmailAddress"));
            IWebElement Passwd = driver.FindElement(By.Name("Passwd"));
            IWebElement PasswdAgain = driver.FindElement(By.Name("PasswdAgain"));
            IWebElement BirthDay = driver.FindElement(By.Name("BirthDay"));
            IWebElement BirthYear= driver.FindElement(By.Name("BirthYear"));
            IWebElement RecoveryPhoneNumber = driver.FindElement(By.Name("RecoveryPhoneNumber"));
            IWebElement RecoveryEmailAddress = driver.FindElement(By.Name("RecoveryEmailAddress"));
            IWebElement submitbutton = driver.FindElement(By.Name("submitbutton"));
            IWebElement iagreebutton = driver.FindElement(By.Name("iagreebutton"));
            //Perform Ops
            FirstName.SendKeys("kkk");
            LastName.SendKeys("lll");
            GmailAddress.SendKeys("vkdqwerty");
            Passwd.SendKeys("lolololo");
            PasswdAgain.SendKeys("lolololo");
            BirthDay.SendKeys("05");
            BirthYear.SendKeys("1999");
            submitbutton.Click();



//SQL Query
select UserId,
(select min(LoginTime) from UserLog where LoginTime in (select Ul.LoginTime from UserLog as Ul where datepart(hh, Ul.LoginTime) >= 02 and Ul.UserId=ULL.UserId) ) as LoginLTTime
,(select max(LogoutTime) from UserLog where LogoutTime in (select Ul.LogoutTime from UserLog as Ul where datepart(hh, dateadd(HOUR, 4, Ul.LogoutTime)) < 06 and Ul.UserId=ULL.UserId) ) as LogoutTime
from UserLog as ULL

group by UserId
