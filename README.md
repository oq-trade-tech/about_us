<p align="center"><img src="oqt_english_logo.png"></p>

## OQ Trading Technology
Headquartered in Brooklyn, New York, OQ Trading Technology is a diverse group of professionals that specializes in connecting traders to the right technology and the right platforms. We use our years of experience in creating complex trading systems to offer unique solutions and customizable software while delivering the highest levels of customer satisfaction.

Contact us at [info@oqtradetech.com](mailto:info@oqtradetech.com) for all inquiries.

### What Makes Us Unique
Our team specializes in creating or tailoring software to meet your specific trading needs

### Experience
Trade with any of the leading Forex brokers we are partnered with. Get immediate access to a huge range of products with several hundred currency pairs and CFDs to choose from. 

### Strategic Partners
Our brokers and education partners have goals consistentand aligned with yours. We want you to succeed. 

### Availability
We are here to help. Our large team of support personnel will assist you with all your trading needs. 

### Quality of Service
Expect a high quality of service from dedicated and highly skilled professionals from our team. We are here to serve you. 

### Cost
Our prices are guaranteed to be competitive. We will work with you to satisfy your pricing requirements.

### Technology
Trade using established platforms such as Metrader, cTrader and Trading Station. Want them automated? Let our expert developers code your next MT4 Expert Advisor or Lua strategy for Marketscope charts in TS2. 

##### Sample Code Snippets

- [Trading Station II](https://github.com/oq-trade-tech/about_us#Trading Station II)
- [MetaTrader 4](https://github.com/oq-trade-tech/about_us#mq4)
- [cTrader](https://github.com/oq-trade-tech/about_us#cTrader)

#### Trading Station
..* Lua sample code

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
#### Mq4

```lua
--[[
Simple signal/slot implementation
]]
local signal_mt = {
    __index = {
        register = table.insert
    }
}
function signal_mt.__index:emit(... --[[ Comment in params ]])
    for _, slot in ipairs(self) do
        slot(self, ...)
    end
end
local function create_signal()
    return setmetatable({}, signal_mt)
end

-- Signal test
local signal = create_signal()
signal:register(function(signal, ...)
    print(...)
end)
signal:emit('Answer to Life, the Universe, and Everything:', 42)

--[==[ [=[ [[
Nested ]]
multi-line ]=]
comment ]==]
[==[ Nested
[=[ multi-line
[[ string
]] ]=] ]==]
```

#### cTrader

```lua
--[[
Simple signal/slot implementation
]]
local signal_mt = {
    __index = {
        register = table.insert
    }
}
function signal_mt.__index:emit(... --[[ Comment in params ]])
    for _, slot in ipairs(self) do
        slot(self, ...)
    end
end
local function create_signal()
    return setmetatable({}, signal_mt)
end

-- Signal test
local signal = create_signal()
signal:register(function(signal, ...)
    print(...)
end)
signal:emit('Answer to Life, the Universe, and Everything:', 42)

--[==[ [=[ [[
Nested ]]
multi-line ]=]
comment ]==]
[==[ Nested
[=[ multi-line
[[ string
]] ]=] ]==]
```

### Site Index
* [OQT Trading Technology website](https://www.oqtradetech.com)
* [OQT Trading Technology Apps Portfolio](https://oq-trade-tech.github.io)

### Leadership Team

[Marco Sierra](https://www.linkedin.com/in/marcosierra1/),
[Alejandra Diaz](https://www.linkedin.com/in/alejandra-diaz-2b973410b/)
