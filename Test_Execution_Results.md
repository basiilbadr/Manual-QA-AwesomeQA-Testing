Summary Scorecard
Total Tests: 20
Passed: 15
Failed: 5
Pass Rate: 75%



Test Suite 1: Account Registration & Security

TC ID	Test Scenario	Priority	Expected Result	Actual Result	Status
REG_01	Valid Registration	High	Account created successfully.	Account created.	PASS
REG_02	Duplicate Email	High	Error: "E-Mail already registered!"	Correct error displayed.	PASS
REG_03	Empty Required Fields	Medium	Error: "Field is required."	Error: "3 to 32 characters."	PASS*
REG_04	Password Masking	High	Input should be hidden (dots).	Characters are masked.	PASS
REG_05	Whitespace Password	Critical	Error: "Password too weak."	Accepted 6 spaces.	FAIL
REG_06	Privacy Policy Bypass	Medium	Blocked until checkbox is ticked.	Correctly blocked.	PASS
REG_07	Phone Data Type	Medium	Error: "Numbers only."	Accepted "ABCDEF".	FAIL


Test Suite 2:	Product Search & Discovery	

TC ID	Test Scenario	Priority	Expected Result	Actual Result	Status	
SRCH_01	Existing Product Search	High	Items (e.g., iPhone) displayed.	Product found.	PASS	
SRCH_02	Non-existent Product	Low	"No products match" message.	Correct message shown.	PASS	
SRCH_03	Empty Search Query	Low	Stay on page or show help msg.	Shown "no match" msg.	PASS	
SRCH_04	Category Navigation	Medium	Clicking "Desktops" shows PCs.	Correct products load.	PASS	
SRCH_05	Currency Toggle	High	Price updates from $ to €/£.	UI updates correctly.	PASS	


Test Suite 3:	Shopping Cart Logic			

TC ID	Test Scenario	Priority	Expected Result	Actual Result	Status
CART_01	Add to Cart (Home)	High	Cart total updates instantly.	Total updated.	PASS
CART_02	Quantity Increase	High	Total price updates (Price x N).	Math is correct.	PASS
CART_03	Remove Item	High	Item deleted; Total is $0.00.	Item removed.	PASS
CART_04	Negative Quantity	Critical	Error: "Invalid Quantity."	Subtracted from total.	FAIL
CART_05	Zero Quantity	Medium	Item not added/removed.	Showed "Success" msg.	FAIL


Test Suite 4: Checkout Flow

CHKT_01	Guest Checkout Flow	High	Proceed without login.	Step-by-step works.	PASS
CHKT_02	Terms & Cond. Bypass	High	Blocked until agreed.	Correctly blocked.	PASS
CHKT_03	Inventory Validation	Critical	Block "Out of Stock" at Add to Cart.	Blocked only at end.	FAIL

