    # MainTestAutomationpr
    import java.util.concurrent.TimeUnit;

    import org.openqa.selenium.By;
    import org.openqa.selenium.WebDriver;
    import org.openqa.selenium.chrome.ChromeDriver;

    public class MyClass {
    public static void main(String[] args) {
      System.setProperty("webdriver.chrome.driver", "C:\\Users\\User\\Desktop\\chromedriver.exe.exe");
        WebDriver driver= new ChromeDriver();
        driver.get("http://automationpractice.com");
        driver.manage().window().maximize();
        driver.findElement(By.className("login")).click();
        driver.findElement(By.id("email_create")).sendKeys("sinacengiz@room.com");
        driver.findElement(By.name("SubmitCreate")).click();
        driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
        driver.findElement(By.id("id_gender1")).click();
        driver.findElement(By.id("customer_firstname")).sendKeys("sina");
        driver.findElement(By.id("customer_lastname")).sendKeys("cengiz");
        driver.findElement(By.id("passwd")).sendKeys("daredevil");
        driver.findElement(By.id("days")).sendKeys("5");
        driver.findElement(By.id("months")).sendKeys("January");
        driver.findElement(By.id("years")).sendKeys("1980");
        driver.findElement(By.id("newsletter")).click();
        driver.findElement(By.id("optin")).click();
        driver.findElement(By.id("company")).sendKeys("esgen yapi denetim");
        driver.findElement(By.id("address1")).sendKeys("nuri duyguer sk. baris apt");
        driver.findElement(By.id("address2")).sendKeys("numara 2 daire 1");
        driver.findElement(By.id("city")).sendKeys("eskisehir");
        driver.findElement(By.id("id_state")).sendKeys("Alabama");
        driver.findElement(By.id("postcode")).sendKeys("00000");
        driver.findElement(By.id("id_country")).sendKeys("United States");
        driver.findElement(By.id("other")).sendKeys("you have amazing clothes mate");
        driver.findElement(By.id("phone")).sendKeys("+234079318993");
        driver.findElement(By.id("phone_mobile")).sendKeys("+75425478965");
        driver.findElement(By.id("alias")).sendKeys("eyup sultan caddesi");
        driver.findElement(By.id("submitAccount")).click();
        driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
        driver.quit();

    }
    }
