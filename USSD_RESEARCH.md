# USSD Service Objectives Research - M-Taka Waste Management

**Date:** November 11, 2025
**Researchers:** Jeff, Adrian, Cynthia
**Objective:** Identify viable USSD use cases for M-Taka waste management system

---

## 1. WASTE SECTOR PLAYERS MAPPING

### 1.1 Waste Generators
**Who they are:**
- Households (individual homes, apartments)
- Businesses (shops, offices, restaurants, hotels)
- Institutions (schools, hospitals, government offices)

**Current role:**
- Generate recyclable waste
- Need collection services
- Receive payment or pay for collection (depending on material value)

**Technology access:**
- Households: Mixed (some have smartphones, some basic phones)
- Small businesses: Mostly have smartphones
- Large institutions: Have computers/smartphones

---

### 1.2 Waste Collectors
**Who they are:**
- Individual pickers (informal sector)
- Community-Based Organizations (CBOs)
- Private waste collection companies
- M-Taka agents

**Current role:**
- Collect waste from generators
- Sort and transport to buyback centers
- Receive payment per kg collected

**Technology access:**
- Individual pickers: Mostly basic phones
- CBO members: Mix of basic and smartphones
- M-Taka agents: Have smartphones (required for agent app)

**Current M-Taka solution:**
- M-Taka Agent App (Android/PWA) - for recording collections, sales, inventory

---

### 1.3 Buyback Centers / Aggregators
**Who they are:**
- Small-scale collection points
- Aggregation centers that consolidate waste

**Current role:**
- Receive waste from collectors
- Sort by material type
- Sell to recovery facilities

**Technology access:**
- Usually have smartphones or computers

**Current M-Taka solution:**
- M-Taka ERP (web) - for managing operations, inventory, finances

---

### 1.4 Recovery Facilities
**Who they are:**
- M-Taka recovery centers (Nairobi, Kisumu, Mombasa)
- Other recycling facilities

**Current role:**
- Process waste materials
- Manage inventory
- Coordinate with agents and buyers

**Technology access:**
- Have computers and smartphones

**Current M-Taka solution:**
- M-Taka ERP (web) - comprehensive management system

---

### 1.5 Buyers/Recyclers
**Who they are:**
- Manufacturing companies
- Export companies
- Processing plants

**Current role:**
- Purchase processed materials
- Recycle into new products

**Technology access:**
- Have computers and smartphones

---

## 2. PROBLEMS EACH PLAYER FACES

### 2.1 Waste Generators Problems

**Communication Issues:**
- ❌ Don't know when waste collector is coming
- ❌ Can't easily request collection service
- ❌ No way to check if their regular collector is available
- ❌ Don't know what materials are accepted
- ❌ Don't know current buying prices

**Information Gap:**
- ❌ No visibility on collection schedules
- ❌ Can't track payment status
- ❌ Don't know which collectors serve their area

---

### 2.2 Waste Collectors Problems

**Operational Challenges:**
- ❌ Can't check inventory levels at buyback center (before traveling there)
- ❌ Don't know current buying prices before collecting
- ❌ Can't confirm if buyback center is open
- ❌ Limited data when internet is unavailable (now solved with offline functionality!)
- ❌ Communication delays with generators

**Route Planning:**
- ❌ Don't know which generators have waste ready for collection
- ❌ Inefficient routing leads to wasted time/fuel

---

### 2.3 Buyback Centers Problems

**Communication:**
- ❌ Can't easily notify collectors when they're at capacity
- ❌ Can't broadcast price changes to collectors
- ❌ Difficult to manage collection schedules

---

### 2.4 Recovery Facilities Problems

**Coordination:**
- ❌ Can't quickly check status of collections across agents
- ❌ Limited real-time visibility when not at computer

---

## 3. EXISTING M-TAKA SOLUTIONS & THEIR LIMITATIONS

### 3.1 M-Taka Agent App (Android/PWA)
**What it does:**
- ✅ Records waste collections from collection points
- ✅ Manages collection points (household, building, institution, business)
- ✅ Tracks collection schedules (which points to visit on which days)
- ✅ Shows daily collection schedule
- ✅ Records sales to buyers (recovery centers or regular buyers)
- ✅ Manages inventory
- ✅ Tracks payments (flat_rate, per_kg, or free)
- ✅ **NOW: Works offline!** (just implemented - can record collections/sales offline)

**Key Data Tracked:**
- Collection points with: name, type, contact (phone), location, payment terms, collection days
- Buyers with: name, contact, location, type
- Collections with: collection point, items (categories + quantities), amount, payment status
- Sales with: buyer, items, total quantity, amount, payment status

**Limitations:**
- ✅ ~~Requires internet~~ (SOLVED - now has offline functionality!)
- Requires smartphone (Android or browser)
- Requires app installation/setup
- Collection points (households/businesses) cannot interact with the system directly

---

### 3.2 M-Taka ERP (Web Application)
**What it does:**
- ✅ Complete management system for recovery centers
- ✅ Manages suppliers (agents who supply waste)
- ✅ Manages customers (manufacturers who buy processed materials)
- ✅ Tracks purchases from suppliers
- ✅ Tracks sales to customers
- ✅ Inventory management (raw materials, processed materials, stock levels, pricing)
- ✅ Material processing workflow (sorting, processing)
- ✅ CRM system (contacts, communication logs, issues/complaints, tasks, analytics)
- ✅ Financial reporting
- ✅ User management

**Key Features:**
- Communication log tracking (call, email, SMS, WhatsApp, meeting, site visit)
- Issue/complaint management linked to suppliers or customers
- Task management for staff
- Detailed analytics and reporting

**Limitations:**
- Requires computer or smartphone with browser
- Requires internet connection
- Not accessible on basic phones
- Primarily for recovery center staff, not waste generators or independent collectors

---

### 3.3 M-Taka Household App (NOT YET DEPLOYED)
**Status:** Planned/In Development

**What it would do:**
- Allow households to request collections
- View collection schedules
- Track payments

**Limitations:**
- Requires smartphone
- Requires internet
- **NOT yet deployed - this is a gap!**

---

## 4. INTERNET ACCESS BARRIERS

### 4.1 Who Faces Internet Barriers?

**Most affected:**
- Households in low-income areas (no smartphones/data)
- Individual waste pickers (basic phones only)
- Rural generators and collectors

**Less affected:**
- M-Taka agents (have smartphones, can use offline mode now)
- Buyback centers (usually have internet)
- Businesses (usually have internet)

### 4.2 When Internet Access is Critical Issue

- **Field workers** moving between areas (inconsistent connectivity)
- **Low-income households** wanting to participate (no smartphones)
- **Emergency situations** when quick communication needed
- **Areas with poor network coverage**

---

## 5. USSD CONSTRAINTS & BEST PRACTICES

### 5.1 What USSD is GOOD for:
✅ Straightforward tasks (1-3 steps)
✅ Information inquiries
✅ Simple transactions
✅ Communication triggers
✅ Works on ALL phones (no smartphone needed)
✅ No internet required
✅ No app installation needed

### 5.2 What USSD is BAD for:
❌ Record keeping (too many fields)
❌ Complex data entry
❌ Tasks requiring multiple screens
❌ Viewing large amounts of data
❌ Tasks requiring images/photos

### 5.3 Successful USSD Examples in Kenya:

**M-PESA (*334#):**
- Send money
- Buy airtime
- Pay bills
- Check balance

**KPLC (*977#):**
- Buy electricity tokens
- Check postpaid balance
- Report outages

**Safaricom (*100#):**
- Buy bundles
- Please call me back
- Check balance

**NHIF (*155#):**
- Check contribution status
- Verify membership

**KRA (*572#):**
- Check PIN status
- Request tax compliance certificate

**Common patterns:**
- Single objective per session
- 2-4 menu levels maximum
- Clear, simple language
- Immediate results/feedback

---

## 5.4 KEY INSIGHT FROM ACTUAL SYSTEM EXPLORATION

**🔍 CRITICAL FINDING:**

After exploring both the ERP and Agent App, I discovered:

1. **Collection schedules ALREADY EXIST** in the agent app
   - Collection points have designated collection days (e.g., Monday, Wednesday)
   - Agents can see which collection points to visit each day
   - Collection points have phone numbers stored in the system

2. **Payment terms ALREADY TRACKED**
   - System knows if collection point pays flat rate, per kg, or free
   - Rates are stored for each collection point

3. **NO DIRECT WAY for collection points to interact with the system**
   - Collection points (households/businesses) cannot check their schedule
   - They cannot confirm if agent is coming
   - They cannot request changes or special collections
   - This is a MAJOR GAP!

**This changes everything for USSD! The best use case is now clear:**
- ✅ Collection points need a way to CHECK their collection schedule
- ✅ Collection points need a way to CONFIRM if collection is happening today
- ✅ Collection points could REQUEST special/emergency collections
- ✅ Agents could CHECK their daily schedule without opening app

---

## 6. POTENTIAL USSD OBJECTIVES FOR M-TAKA (UPDATED WITH REAL INSIGHTS)

### 🏆 Option 1: Collection Schedule Checker (COLLECTION POINTS) **[NEW - BASED ON REAL SYSTEM]**

**Who:** Collection points (households, businesses, institutions, buildings) that are already in the M-Taka system

**Problem Solved:**
- Don't know which day agent will come
- Forget their collection schedule
- Can't confirm if today is their collection day
- Waste is ready but unsure if agent is coming

**How it works:**
```
Dial *XXX#
1. Check Collection Schedule
   - Enter phone number (registered in system)
   - See: Next collection date
   - See: Collection days (e.g., "Every Monday & Thursday")
   - See: Agent name/contact
   - Optional: Request SMS reminder
```

**Backend Requirements:**
- ✅ Data ALREADY EXISTS in agent app!
- ✅ Collection points have phone numbers
- ✅ Collection days are tracked
- ✅ Agent info is available
- Just need API endpoint to query by phone number

**Pros:**
- ✅ Solves real problem - collection points currently have NO way to check schedule
- ✅ Very simple (2-3 steps)
- ✅ Uses EXISTING data - minimal backend changes
- ✅ Works for collection points without smartphones
- ✅ Reduces missed collections (points prepare waste on time)
- ✅ Reduces unnecessary calls to agents

**Cons:**
- Only works for collection points already registered in system
- Requires phone number matching (must use registered number)

**Impact:**
- HIGH - Fills major gap in current system
- Improves collection point experience
- Reduces agent workload (fewer "when are you coming?" calls)

---

### Option 2: Emergency Collection Request (COLLECTION POINTS) **[NEW]**

**Who:** Households, businesses wanting collection

**Problem Solved:**
- Hard to contact waste collector
- Don't know who to call
- No smartphone to use app

**How it works:**
```
Dial *XXX#
1. Request Collection
   - Enter phone number
   - Select waste type (1=Plastic, 2=Paper, etc)
   - Confirm location/area
   - System notifies nearest agent
   - Receive SMS confirmation with agent contact
```

**Main product:** Household app (not yet deployed)
**USSD alternative:** When no smartphone available

**Pros:**
- Very simple (3-4 steps)
- Solves real problem
- Increases M-Taka reach to non-smartphone users
- Helps agents get more collections

**Cons:**
- Requires system to find "nearest agent" (backend logic needed)
- Requires agent notification system

---

### Option 2: Price Inquiry Service (WASTE COLLECTORS)

**Who:** Waste pickers, collectors

**Problem Solved:**
- Don't know current buying prices
- Can't decide if worth collecting certain materials
- Prices change frequently

**How it works:**
```
Dial *XXX#
1. Check Prices
   - Select material type
   - See current price per kg
   - See which center is buying
```

**Main product:** Agent app (shows prices)
**USSD alternative:** For pickers without smartphones

**Pros:**
- Very simple (2-3 steps)
- Useful information
- Encourages more collections

**Cons:**
- Limited value (just info, no action)
- Prices may vary by location

---

### Option 3: Buyback Center Status Check (WASTE COLLECTORS)

**Who:** Waste collectors before traveling to center

**Problem Solved:**
- Waste time traveling to full/closed centers
- Don't know operating hours
- Can't confirm center is accepting materials

**How it works:**
```
Dial *XXX#
1. Check Center Status
   - Select nearest center
   - See: Open/Closed
   - See: Accepting materials (Yes/No)
   - See: Operating hours
```

**Main product:** None currently
**USSD alternative:** New service

**Pros:**
- Saves collectors time and transport costs
- Simple query (2 steps)

**Cons:**
- Requires real-time center status updates
- Limited centers currently

---

### Option 4: Collection Schedule Inquiry (WASTE GENERATORS)

**Who:** Households/businesses with scheduled pickups

**Problem Solved:**
- Forget collection day
- Don't know what time collector comes
- Can't plan waste separation

**How it works:**
```
Dial *XXX#
1. Check My Schedule
   - Enter phone number
   - See next collection date
   - See material types collected
   - Receive SMS reminder
```

**Main product:** Household app (planned)
**USSD alternative:** For basic phone users

**Pros:**
- Helps generators prepare waste
- Reduces missed collections
- Simple (2-3 steps)

**Cons:**
- Requires scheduled collection system
- Only useful for regular customers

---

### Option 5: Agent Availability Check (WASTE GENERATORS)

**Who:** Households wanting to know if agent is working today

**Problem Solved:**
- Don't know if regular collector is available
- Waste prepared but no collection happens

**How it works:**
```
Dial *XXX#
1. Check Agent Availability
   - Enter agent code/number
   - See: Available today (Yes/No)
   - See: Expected time in your area
   - Option to request callback
```

**Main product:** None
**USSD alternative:** New communication service

**Pros:**
- Improves communication
- Reduces missed collections

**Cons:**
- Requires agents to update availability
- May be complex to implement

---

## 7. EVALUATION CRITERIA

For each objective, we evaluate:

| Criteria | Weight | What to Check |
|----------|--------|---------------|
| **Simplicity** | HIGH | Can be done in 2-4 steps? |
| **Real Problem** | HIGH | Solves actual pain point? |
| **Feasibility** | HIGH | Can we build backend logic? |
| **Reach** | MEDIUM | How many users affected? |
| **Value** | MEDIUM | Impact on operations? |
| **Uniqueness** | LOW | Different from competitors? |

---

## 8. UPDATED RECOMMENDATIONS (BASED ON REAL SYSTEM EXPLORATION)

### 🥇 TOP RECOMMENDATION: Collection Schedule Checker

**Why this is the best option:**

1. **Fills a REAL gap** - Collection points currently have NO way to check their schedule
2. **Uses EXISTING data** - All needed data already in system (phone numbers, schedules, agent info)
3. **Minimal development** - Just need one API endpoint to query collection points by phone
4. **Very simple USSD** - Only 2-3 steps
5. **High impact** - Improves experience for ALL collection points (hundreds/thousands of users)
6. **Reduces agent workload** - Fewer calls asking "when are you coming?"
7. **Increases collections** - Points prepare waste on time when they know schedule

**Implementation Priority:** ⭐⭐⭐⭐⭐ (5/5)

---

### 🥈 SECOND CHOICE: Emergency Collection Request

**Pros:**
- Solves problem for one-time/new users
- Expands M-Taka reach
- Generates new business

**Cons:**
- Requires agent notification system (more complex)
- May overwhelm agents with requests
- Harder to manage than scheduled collections

**Implementation Priority:** ⭐⭐⭐ (3/5)

---

### 🥉 THIRD CHOICE: Agent Daily Schedule Checker

**Pros:**
- Helps agents check schedule without opening app
- Very simple
- Uses existing data

**Cons:**
- Low priority - agents already have app
- Agents already can see schedule in app
- App now works offline

**Implementation Priority:** ⭐⭐ (2/5)

---

### NOT RECOMMENDED (for now):

**Price Inquiry Service:**
- ❌ Low impact - prices don't change frequently
- ❌ Limited users - only for informal pickers
- ❌ Agents already can see prices in app

**Buyback Center Status:**
- ❌ Limited centers currently
- ❌ Most collectors already know center hours
- ❌ Low priority vs collection schedule

---

## 9. IMPLEMENTATION PLAN FOR TOP RECOMMENDATION

### Phase 1: Backend API Development (1-2 days)

**New API Endpoint Needed:**
```
GET /agents/collection-points/schedule/?phone_number={number}

Response:
{
  "collection_point": {
    "name": "ABC Supermarket",
    "type": "business",
    "location": "Nairobi, Westlands"
  },
  "collection_days": [
    {"day": "Monday", "display": "Mon"},
    {"day": "Thursday", "display": "Thu"}
  ],
  "next_collection": "2025-11-14",
  "agent": {
    "name": "John Kamau",
    "phone": "+254712345678"
  },
  "payment_terms": "per_kg",
  "rate": "50.00"
}
```

**Changes Needed:**
- Add phone number lookup in collection points table
- Calculate next collection date based on current date + collection days
- Return agent info associated with collection point

---

### Phase 2: USSD Menu Design

```
*XXX# (Main Menu)
1. Check Collection Schedule
2. Contact Agent
3. Report Issue
0. Exit

User selects: 1

Enter your phone number:
> 0712345678

[System checks database]

YOUR COLLECTION SCHEDULE
------------------------
Name: ABC Supermarket
Next Collection: Thursday, Nov 14
Regular Days: Mon & Thu
Agent: John Kamau
Tel: 0712345678

1. SMS me this info
2. Contact agent
0. Main menu
```

---

### Phase 3: USSD Gateway Integration

**Options in Kenya:**
- Africa's Talking
- Safaricom USSD Gateway
- Twilio (if available)

**Requirements:**
- USSD short code application (*XXX#)
- API integration for menu handling
- SMS gateway for notifications

---

### Phase 4: Testing & Rollout

1. **Internal Testing** (3-5 days)
   - Test with M-Taka staff
   - Verify all collection points can be found by phone
   - Test edge cases (no phone, wrong number, etc.)

2. **Pilot with Select Collection Points** (1-2 weeks)
   - Choose 20-50 collection points
   - Notify them about the USSD service
   - Collect feedback

3. **Full Rollout**
   - SMS all collection points with USSD code
   - Add USSD code to collection receipts
   - Train agents to promote USSD service

---

## 10. QUESTIONS FOR TEAM DISCUSSION

### Technical Questions:
1. ✅ **Do we have phone numbers for all collection points?** - YES (confirmed in agent app)
2. ✅ **Are collection schedules tracked?** - YES (collection_days field exists)
3. ❓ **Which USSD gateway should we use?** - Africa's Talking vs Safaricom
4. ❓ **Do we need approval for USSD short code?** - Check with Safaricom
5. ❓ **What's the estimated cost per USSD session?** - Usually KES 0.50 - 2.00

### Business Questions:
1. **Should collection points pay for USSD?** - Probably FREE (M-Taka absorbs cost)
2. **How do we notify collection points about USSD?** - SMS campaign + agent communication
3. **Should we expand to non-registered collection points?** - Phase 2 feature
4. **What other info should USSD provide?** - Payment status? Collection history?

### Priority Questions:
1. ✅ **Is this the right first USSD feature?** - YES - fills major gap with minimal effort
2. **Should we do this before household app?** - YES - much simpler, uses existing data
3. **Timeline for implementation?** - 2-3 weeks realistic?

---

## 11. CONCLUSION

After thorough exploration of the actual M-Taka systems (ERP and Agent App), the **Collection Schedule Checker USSD service** emerges as the clear winner because:

1. **Real Problem** - Collection points have no way to check their schedule currently
2. **Real Data** - All needed information already exists in the system
3. **Real Impact** - Helps hundreds/thousands of collection points
4. **Real Simplicity** - Only 2-3 USSD steps needed
5. **Real Feasibility** - Minimal backend development required

This is a **quick win** that delivers high value with low effort.

**Recommended Decision: Proceed with Collection Schedule Checker USSD**

---

**Document Status:** Ready for team review
**Next Update:** After team discussion (November 12, 2025)
**Prepared by:** Jeff (with exploration of actual M-Taka systems)
