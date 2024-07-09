# First-project
this is for practice

System.setProperty("webdriver.chrome.driver","C:\\Users\\VISWA\\eclipse-workspace\\selenium\\Driver\\chromedriver.exe");
		WebDriver dd = new ChromeDriver();
		dd.get("https://www.amazon.in/");
		dd.manage().window().maximize();
		//mouse based Actions
		
		Actions ac = new Actions(dd);       
		                                               //normalize-space method
		WebElement elect = dd.findElement(By.xpath("//a[normalize-space()='New Releases']"));
		ac.click(elect).build().perform();
	//	ac.contextClick(elect).build().perform();
	//	ac.doubleClick(elect).build().perform();
	//	ac.moveToElement(elect).build().perform();	 
		ac.contextClick().build().perform();	
			
		ac.clickAndHold(elect).build().perform();
		ac.moveToElement(elect, 0, 0);
		
