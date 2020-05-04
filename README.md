<p align="center"><img src="oqt_english_logo.png"></p>

## OQ Trading Technology
Headquartered in Brooklyn, New York, OQ Trading Technology is a diverse group of professionals that specializes in connecting traders to the right technology and the right platforms. We use our years of experience in creating complex trading systems to offer unique solutions and customizable software while delivering the highest levels of customer satisfaction.

Contact us at [info@oqtradetech.com](mailto:info@oqtradetech.com) for all inquiries.

### What Makes Us Unique
Our team specializes in creating or tailoring software to meet your specific trading needs

### Experience
Trade with any of the leading Forex brokers we are partnered with. Get immediate access to a huge range of products with several hundred currency pairs and CFDs to choose from. 

### Strategic Partners
Our brokers and education partners have goals consistent and aligned with yours. We want you to succeed. 

### Availability
We are here to help. Our large team of support personnel will assist you with all your trading needs. 

### Quality of Service
Expect a high quality of service from dedicated and highly skilled professionals from our team. We are here to serve you. 

### Cost
Our prices are guaranteed to be competitive. We will work with you to satisfy your pricing requirements.

### Technology
Trade using established platforms such as Metrader, cTrader and Trading Station. Want them automated? Let our expert developers code your next MT4 Expert Advisor or Lua strategy for Marketscope charts in TS2. 

##### Sample Code Snippets

- [Trading Station II](https://github.com/oq-trade-tech/about_us#TS2-lua)
- [MetaTrader 4](https://github.com/oq-trade-tech/about_us#MT4-mq4)
- [cTrader](https://github.com/oq-trade-tech/about_us#cTrader)

#### TS2-lua
  * Lua sample code

```lua
function addOrderAlert(orderID, key, data)
	if not containsKey(alertsOrder, orderID) then
		alertsOrder[orderID] = {};
	end
	alertsOrder[orderID][key] = data;
end

function addTradeAlert(tradeID, key, data)
	if not containsKey(alertsTrade, tradeID) then
		alertsTrade[tradeID] = {};
	end
	alertsTrade[tradeID][key] = data;
end

function sendAlerts()
	local messages = formatAlerts();
	if instance.parameters.advanced_alert_key ~= "" and instance.parameters.use_advanced_alert then
		sendTelegram(messages);
	end
	alertsOrder = {};
	alertsTrade = {};
end
```
#### MT4-mq4
  * MetaTrader 4 mq4 sample code

```lua
   for(int i = 0; i < 5; i++) {
      if(Wr[i] >= -20){
         DownArrow(40 * i + pix + 50, 120, n);
      }
      if(Wr[i] <= -80){
         UpArrow(40 * i + pix + 50, 120, n);
      }
      if((Wr[i] < -20) && (Wr[i] > -80)){
         RightArrow(40 * i + pix + 50, 120, n);
      }
      n++; 
   }
```

#### cTrader
  * C# for cTrader

```C#
	{ 
		if (TimeFrame <= TimeFrame.Hour)
    		PivotTimeFrame = TimeFrame.Daily;
    		else if (TimeFrame < TimeFrame.Daily)
    		{
    			PivotTimeFrame = TimeFrame.Weekly;
    		}
    		else
    			PivotTimeFrame = TimeFrame.Monthly;
 
 
    		Enum.TryParse(PivotColor, out pivotColor);
    		Enum.TryParse(SupportColor, out supportColor);
    		Enum.TryParse(ResistanceColor, out resistanceColor);
 
 	}
```

### Site Index
* [OQT Trading Technology website](https://www.oqtradetech.com)
* [OQT Trading Technology Apps Portfolio](https://oq-trade-tech.github.io)

### Leadership Team

[Marco Sierra](https://www.linkedin.com/in/marcosierra1/),
[Alejandra Diaz](https://www.linkedin.com/in/alejandra-diaz-2b973410b/)
