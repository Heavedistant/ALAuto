## Using Config.ini
Setting up Config.ini will tell ALAuto which map to run combat in and how to handle ship retirement, mission rewards, and more.

### [Network]
**Service:** Configure your ADB server ip and port here, example **Service: 192.168.0.2:5037**. Alternatively leave as **Service: IP:PORT** to default to 127.0.0.1:5037.

### [Combat]
Setup which map ALAuto will run combat in here.  

**Enabled:** ALAuto will navigate from the main menu to the map you specify.  
Options: **True** to enable the combat cycle. **False** to disable combat.  
Example: **Enabled: True**

**Map:** Supported standard maps 1-1 through 8-4. Additional map names and events supported are A1 to D4 and *The Pursuit of Graf Spree* E-SP1 to E-SP3.  
Examples: **Map: 3-4** or **Map: E-SP2**  

**RetireCycle:** How many times ALAuth will complete combat of a map before navigating to the Retire menu to retire common and rare ships only. Elite and above ships will never be retired.  
Example: **RetireCycle: 2**  

### [Modules]
This section is for configuring ALAuto quality of life features.  

**Commisions:** ALAuto will automatically populate and start commisions.  
Options: **True** enable automatically accepting and completing commisions. **False** do not automatically accept or complete commisions.  
Example: **Commisions: False**

**Enhancement**: ALAuto will use common ships as enhancements instead of retiring them. Options: **True** enhance fleet with common ships. **False** do not use common ships to enhance fleet.  
Example: **Enhancement: False**

**Missions:** ALAuto will accept missions rewards automatically.  
Options: **True** receive rewards from missions automatically when they become available. **False** do not automatically accept missions rewards.  
Example: **Missions: True**

**Retirement:** ALAuto will use the Ship Build Retire menu to retire common and rare ships every RetireCycle (described above). Options: **True** enable retiring common and rare ships. **False** do not automatically retire common and rare ships.  
Note: without setting this to true, your ship dock will quickly fill up and prevent you from continuing combat.  
Example: **Retirement: True**

### [Events]
This section provides support for certain in-game events. Currently supports **Crosswave** only.  

**Enabled:** ALAuto will navigate to the Crosswave event and run combat on the maps you choose.  
Options: **True** run combat in Crosswave event levels. **False** do not run combat in Crosswave event levels.  
Example: **Enabled: False**

**Event:** Specify the event name to run combat in.  
Note: some events may be supported in the **[Combat]** section, described above. See the map names for more detail. Support for additional events may be added here in the future.  
Example: **Event: Crosswave**  

**Levels:** Crosswave maps supported by difficulty level.
Options: **E** Easy, **N** Normal, **H** Hard, **EX** E.X.  
Examples: **Levels: E,N** or **Levels: N,H,EX**  
