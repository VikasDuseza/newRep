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
