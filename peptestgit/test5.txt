package pom.peptestgit;
import java.util.HashMap;
import java.util.List;
import org.openqa.selenium.By; 
import org.openqa.selenium.WebElement; 
import org.openqa.selenium.support.ui.ExpectedConditions; 
import org.openqa.selenium.support.ui.WebDriverWait; 
import com.prolifics.ProlificsSeleniumAPI;
import org.openqa.selenium.Keys; 
import org.testng.annotations.Parameters; 
import org.testng.annotations.BeforeClass; 
import org.testng.annotations.Test; 
import org.testng.annotations.AfterClass; 
import org.openqa.selenium.Alert; 
import org.openqa.selenium.JavascriptExecutor;
import java.io.File;
import java.io.FileInputStream;
import java.io.FileNotFoundException;
import java.io.FileOutputStream;
import java.io.IOException;
import java.io.InputStream;
import java.util.Properties;


public class EmployeesPEP11
{
	ProlificsSeleniumAPI oPSelFW;
	String currentWindow="";
	String flag="";
	static Properties properties = new Properties();
	
	 static Properties prop = new Properties();
	   

	public  EmployeesPEP11(ProlificsSeleniumAPI oPSelFW)
	{
		this.oPSelFW = oPSelFW;
		currentWindow = oPSelFW.driver.getWindowHandle();
	}

	
	public void  EC_PeptestGit_EmployeesPEP11(String webserviceURL,String sDOADataSetId,String sDOAStepNo, String strEffectaOutKeyDataService,String sEffectaParameters) throws Exception 
	{
		webserviceURL=webserviceURL+"/6917";
		oPSelFW.sDOAStepNumberReport=sDOAStepNo;
		oPSelFW.setEffectaParametersInPOMLevel(sEffectaParameters);

flag=oPSelFW.checkForFrames("id=EmployeeEmailOfficial&&id=EmployeeEmailOfficial&&name=data[Employee][email_official]&&css=#EmployeeEmailOfficial&&xpath=//input[@id='EmployeeEmailOfficial']&&xpath=//form[@id='EmployeeLoginForm']/div[2]/input&&xpath=//div[2]/input", currentWindow); 
oPSelFW.prolifics("clickAndWait",  "id=EmployeeEmailOfficial&&id=EmployeeEmailOfficial&&name=data[Employee][email_official]&&css=#EmployeeEmailOfficial&&xpath=//input[@id='EmployeeEmailOfficial']&&xpath=//form[@id='EmployeeLoginForm']/div[2]/input&&xpath=//div[2]/input", "EmployeeEmailOfficial"); 


	flag=oPSelFW.checkForFrames("id=EmployeeEmailOfficial&&id=EmployeeEmailOfficial&&name=data[Employee][email_official]&&css=#EmployeeEmailOfficial&&xpath=//input[@id='EmployeeEmailOfficial']&&xpath=//form[@id='EmployeeLoginForm']/div[2]/input&&xpath=//div[2]/input", currentWindow); 
oPSelFW.prolifics("typeSpecifiedText","id=EmployeeEmailOfficial&&id=EmployeeEmailOfficial&&name=data[Employee][email_official]&&css=#EmployeeEmailOfficial&&xpath=//input[@id='EmployeeEmailOfficial']&&xpath=//form[@id='EmployeeLoginForm']/div[2]/input&&xpath=//div[2]/input" ,oPSelFW.getTestDataEffectaWebservices(webserviceURL, "EmployeeEmailOfficial") , "EmployeeEmailOfficial"); 



	flag=oPSelFW.checkForFrames("css=.clearfix:nth-child(5)&&css=.clearfix:nth-child(5)&&xpath=//body/div/div/div[3]", currentWindow); 
oPSelFW.prolifics("clickAndWait",  "css=.clearfix:nth-child(5)&&css=.clearfix:nth-child(5)&&xpath=//body/div/div/div[3]", "clearfixnth-child5"); 


	flag=oPSelFW.checkForFrames("id=EmployeeHashCode&&id=EmployeeHashCode&&name=data[Employee][hash_code]&&css=#EmployeeHashCode&&xpath=//input[@id='EmployeeHashCode']&&xpath=//form[@id='EmployeeLoginForm']/div[3]/input&&xpath=//div[3]/input", currentWindow); 
oPSelFW.prolifics("clickAndWait",  "id=EmployeeHashCode&&id=EmployeeHashCode&&name=data[Employee][hash_code]&&css=#EmployeeHashCode&&xpath=//input[@id='EmployeeHashCode']&&xpath=//form[@id='EmployeeLoginForm']/div[3]/input&&xpath=//div[3]/input", "EmployeeHashCode"); 


	flag=oPSelFW.checkForFrames("id=EmployeeHashCode&&id=EmployeeHashCode&&name=data[Employee][hash_code]&&css=#EmployeeHashCode&&xpath=//input[@id='EmployeeHashCode']&&xpath=//form[@id='EmployeeLoginForm']/div[3]/input&&xpath=//div[3]/input", currentWindow); 
oPSelFW.prolifics("typeSpecifiedText","id=EmployeeHashCode&&id=EmployeeHashCode&&name=data[Employee][hash_code]&&css=#EmployeeHashCode&&xpath=//input[@id='EmployeeHashCode']&&xpath=//form[@id='EmployeeLoginForm']/div[3]/input&&xpath=//div[3]/input" ,oPSelFW.getTestDataEffectaWebservices(webserviceURL, "EmployeeHashCode") , "EmployeeHashCode"); 



	flag=oPSelFW.checkForFrames("id=submitBtn&&id=submitBtn&&css=#submitBtn&&xpath=//button[@id='submitBtn']&&xpath=//form[@id='EmployeeLoginForm']/div[7]/label/div/button&&xpath=//button&&xpath=//button[contains(.,' ')]", currentWindow); 
oPSelFW.prolifics("verifyText","id=submitBtn&&id=submitBtn&&css=#submitBtn&&xpath=//button[@id='submitBtn']&&xpath=//form[@id='EmployeeLoginForm']/div[7]/label/div/button&&xpath=//button&&xpath=//button[contains(.,' ')]" ," "); 


	}


}
