```markdown
# CS2 Case Bot - Detailed Setup Guide

**Created by Mk4gtiguy**

## Prerequisites

- [Streamer.bot](https://streamer.bot) v1.0.4 or higher installed
- Your streaming platform connected (Twitch, YouTube, or Trovo)

---

## Step 1: Add Persisted Globals (Skin Lists)

1. Open Streamer.bot
2. Go to **Services** → **Global Variables** → **Persisted Globals**
3. Open `persisted-globals.txt` from this repo
4. Copy each line (one at a time) and click **Add New Variable**
5. Paste the name and value
6. Repeat for all 36 skin lists

---

## Step 2: Create Actions

For each command, follow these steps:

### 2.1 Create the Action
1. Right-click in Actions panel → **Add Action**
2. Name it (e.g., `Case_Command`)

### 2.2 Add C# Code
1. Click **Add Sub-Action** → **Core** → **C# Code**
2. Paste the code from `V1.3-Complete-Code-Reference.md`
3. Click **Compile** (should show no errors)

### 2.3 Set Trigger
1. Click **Triggers** tab
2. Click **Add Trigger** → **Command**
3. Enter the command name (e.g., `!case`)

### 2.4 Special: Case_Command Sub-Action
For the `!case` command only:
1. After the C# code, click **Add Sub-Action**
2. Select **Core** → **Actions** → **Run Action**
3. Select `CS2_OpenCase` as the target

---

## Step 3: Required Actions List

| Action Name | Command | Special Notes |
|-------------|---------|---------------|
| CS2_OpenCase | (none) | Sub-Action only |
| SetCase_Command | `!setcase` | |
| Case_Command | `!case` | Must run CS2_OpenCase as Sub-Action |
| Inv_Command | `!inv` | |
| Sell_Command | `!sell` | |
| Balance_Command | `!balance` | |
| Daily_Command | `!daily` | |
| Tradeup_Command | `!tradeup` | |
| Jackpot_Command | `!jackpot` | |
| JackpotInfo_Command | `!jackpotinfo` | |
| Jackpot_Draw | `!jackpotdraw` | Set permission to Mods only |
| MyStats_Command | `!mystats` | |
| CaseStats_Command | `!casestats` | |
| CaseInfo_Command | `!caseinfo` | |
| Odds_Command | `!odds` | |
| InventoryValue_Command | `!inventoryvalue` | |
| TopInventory_Command | `!topinventory` | |
| TopMoney_Command | `!topmoney` | |
| TopGolds_Command | `!topgolds` | |
| TopOpens_Command | `!topopens` | |
| Help_Command | `!help` | |

---

## Step 4: Set Mod Permission for Jackpot Draw

1. Find `Jackpot_Draw` action
2. Click **Triggers** tab
3. Click the trigger → Set **Permission** → **Moderator**

---

## Step 5: Test Your Bot

In your chat, type:

```

!help
!setcase Dreams
!balance
!daily
!case
!inv

```

If everything works, you're ready to go!

---

## Troubleshooting

### "CPH does not contain a definition for 'GetArg'"
- Use `args["rawInput"].ToString()` instead

### Case won't switch
- Use `!setcase Dreams` not `!case Dreams`

### Jackpot not working
- Ensure `!jackpotdraw` is mods only
- Check that `JackpotPot` and `JackpotEntries` globals exist

### Balance always $0
- Run `!daily` first to get starting money

---

## Need Help?

- Open an issue on GitHub
- Join the Streamer.bot Discord

---

## Support

If this bot helps your stream, consider supporting me on Ko-fi:

https://ko-fi.com/mk4gtiguy
```