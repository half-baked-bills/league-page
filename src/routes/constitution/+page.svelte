<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneTwoOne, oneTwoTwo, oneTwoThree, oneTwoFour, oneTwoFive, oneThree;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne;
    let six, sixOne, sixTwo, sixThree;
    let seven, sevenOne, sevenTwo, sevenThree;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">Average Joe's League Constitution</h1>
    <p> The golden rule - Don't be a dick. Shit-talking and regular sportsmanlike banter is fine but no racism or bigotry will be tolerated. One warning before being ejected with no refund for repeat violation of this rule.</p>
    
    <h2 class="noUnderscore">Table of Contents</h2>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(one)}>Section 1: Roster</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneOne)}>1.1 Positional Breakdown</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneTwo)}>1.2 Trading</h4>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoThree)}>1.2.3 Trade Deadline</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoFour)}>1.2.4 Trade Restrictions</h5>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneThree)}>1.3 Waiver Wire</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(two)}>Section 2: Drafting</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoOne)}>2.1 Draft Order</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoTwo)}>2.2 Rookie Drafts</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(three)}>Section 3: Scoring System</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(threeOne)}>3.1 Voting on Scoring System</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(four)}>Section 4: Postseason</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourOne)}>4.1 Playoffs</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourTwo)}>4.2 Playoff Tiebreakers</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourThree)}>4.3 Empire Rule</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(five)}>Section 5: Tanking Policy</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fiveOne)}>5.1 League Tanking Policy</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(six)}>Section 6: Replacing Managers</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixOne)}>6.1 Removing Managers</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixTwo)}>6.2 Replacing Managers</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixThree)}>6.3 Replacement Incentive</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(seven)}>Section 7: League Finances</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenOne)}>7.1 League Dues</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixTwo)}>7.2 Payout</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixThree)}>7.3 Raising Dues</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(eight)}>Section 8: League Changelog</h3>
    
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1 - Roster Breakdown</h2>
    
    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 Positional Breakdown</h3>
        
    <p class="underscore">Starters</p>
    <ul>
        <li>QB</li>
        <li>RB</li>
        <li>RB</li>
        <li>WR</li>
        <li>WR</li>
        <li>TE</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>SUPERFLEX (QB/WR/RB/TE)</li>
    </ul>
    
    <p>11 Bench Spots (Expanded to 15 between the league draft and start of regular season)</p>

    <p>2 IR Spots (Player must be labeled as IR, Out, or Covid in the Sleeper App)</p>

    <p>4 Taxi Squad Spots (Can only store players with less than 2 years of experience, locks at start of season)</p>
        


    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 Trading</h3>
    
    <p>Trading of players and draft picks (up to 3 drafts away) are allowed. There are no trade vetos, the commissioner is the only person who can veto a trade in the event of obvious collusion. Tradable assets include players, draft picks, and FAAB $.</p>
    
    
    <h4 bind:this={oneTwoThree}>1.2.3 Trade Deadline</h4>
    <div class="subBlock">
        <p>The trade deadline is set for the 13th week of the NFL season. Once the 13th week has completed, no trades will be processed until after the playoffs have been decided.</p>
    </div>
    
    <h4 bind:this={oneTwoFour}>1.2.4 Trade Restrictions</h4>
    <div class="subBlock">
        <p>You will not be able to trade draft picks that are more than 3 drafts away. For example, during the 2025 season you cannot trade any picks in or after the 2029 season. You may only trade FAAB $ from the current season.</p>

        <p>If you trade your team's future season 1st or 2nd round picks, you will be responsible for paying your league dues for that season within 7 days of the trade date (for example, if the current season is 2025 and you trade away your 2027 first rounder, you will need to pay your league dues for 2026 and 2027 within 7 days). If you leave the league, you forfeit the money already paid and it will be donated to the incoming manager's account that assumes control of your orphaned team.</p>
    </div>
    
    
    
    <h3 bind:this={oneThree}>1.3 Waiver Wire</h3>
    
    <p>Each team will begin the regular season with $150 FAAB dollars that you can use to obtain free agent players. $0 bids are allowed.</p>

    <p>At the end of the regular season once a champion has been crowned, the FAAB budget will reset (use it or lose it).</p>

    <p>During the off season, each team will be given $50 FAAB to use. Any remaining total will be added to the regular season $150 if not used.</p>
    


    <h2 class="sectionHeading" bind:this={two}>Section 2 - Drafting</h2>
    
    <h3 bind:this={twoOne}>2.1 Draft Order</h3>
    <p>The rookie draft order will be decided by team reverse max points for. The bottom six teams will be assigned draft picks 1-6 based on their max PF value of the regular season only, with the lowest scoring team assigned the first overall pick.
    The top six playoff teams will be assigned draft position as follows: </p>
    <ul>
        <li>League champion, 12th pick</li>
        <li>Second place, 11th pick</li>
        <li>3rd and 4th place, 9th and 10th picks based on regular season reverse max PF</li>
        <li>5th and 6th place, 7th and 8th picks base on regular season reverse max PF</li>
    </ul>

    <h3 bind:this={twoTwo}>2.2 Rookie Drafts</h3>
    <p>Rookie drafts will consist of 4 rounds of drafting, with unlimited time for each pick. To make room for the incoming players, benches will be expanded by (4) spots at the conclusion of the rookie draft. These spots will be removed before the start of the regular season, at which point you will need to have cut the necessary players.</p>
    <p>Any spots not filled during the draft, can be filled immediately afterwards from the waiver wire.</p>
    
    
    <h2 class="sectionHeading" bind:this={three}>Section 3 - Scoring System</h2>

    <h3 bind:this={threeOne}>3.1 Scoring System</h3>
    <p>The league scoring system breakdown is listed on the Sleeper fantasy app (for the most part, it follows typical .5PPR Scoring). The scoring system will never change without a majority league vote.</p>



    <h2 class="sectionHeading" bind:this={four}>Section 4 - Postseason</h2>
    
    <h3 bind:this={fourOne}>4.1 Playoffs</h3>
    <p>At the end of the season, 6 teams will make the playoffs. The first round of playoffs will commence in week 15. The top two seeded teams will earn a bye week for the first round of playoffs.</p>
    
    <h3 bind:this={fourTwo}>4.2 Seeding Tiebreakers</h3>
    <p>If two teams finish with the same regular season record, the tiebreakers will go as follows:</p>

    <ol>
        <li>Points For</li>
        <li>Head 2 Head Record</li>
        <li>Total Points Against</li>
        <li>Coin Flip</li>
        <li>Duel to the death</li>
    </ol>

    <h3 bind:this={fourThree}>4.3 Empire Rule</h3>
    <p>If the same team/manager wins three consecutive years in a row, it will trigger an automatic full league redraft the following season.</p>


    <h2 class="sectionHeading" bind:this={five}>Section 5 - Tanking Policy</h2>
    
    <h3 bind:this={fiveOne}>5.1 League Tanking Policy</h3>
    <p>Our draft positions are based on max PF, so leaving your roster empty does you no good in the long run. Please set a full lineup if you are able to do so to keep the league competitve. If you truely want to tank for draft position, the best way to do that is to trade away the players on your roster scoring points.</p>


    <h2 class="sectionHeading" bind:this={six}>Section 6 - Replacing Managers</h2>
    
    <h3 bind:this={sixOne}>6.1 Removing Managers</h3>
    <p>Short of continuously failing to set a valid lineup, or confirmed collusion, no manager can be removed against their will. Participation, through the league chat, trade offers, and the waiver wire, is strongly encouraged but generally not grounds for removal.</p>
    
    <h3 bind:this={sixTwo}>6.2 Replacing Managers</h3>
    <p>When a manager needs to be replaced, the commisioner will try to find a suitable candidate with some connection to at least a portion of the existing managers. Priority will be placed on managers who are eager to take on a dynasty commitment and will be very active within the league.</p>
    
    <h3 bind:this={sixThree}>6.3 Replacement Incentive</h3>
    <p>In the event that a manager chooses to quit the league or is removed by a comissioner, the replacement manager will be granted all dues already paid by the leaving manager.</p>


    <h2 class="sectionHeading" bind:this={seven}>Section 7 - League Finances</h2>
    
    <h3 bind:this={sevenOne}>7.1 League Dues</h3>
    <p>League dues are set at $40 per season and will always be paid for one season in advance. Dues are collected through leaguesafe and a link to the latest leaguesafe account will be provided. All managers must be fully paid up before the start of the rookie draft.</p>
    
    <h3 bind:this={sevenTwo}>7.2 Payout</h3>
    <p>League payout is structured as follows, total pot: $480</p>
    <ul>
        <li>1st place: $290</li>
        <li>2nd place: $120</li>
        <li>3rd place: $50</li>
        <li>admin fees (trophies, plates, website): $20</li>
    </ul>
    
    <h3 bind:this={sevenThree}>7.3 Raising Dues & Changing League Rules</h3>
    <p>A 7/12th majority vote is required in order to raise league dues, change a current league rule, or implement a new league rule. In the event that a manager is no longer financially comfortable with the buyin, finding a co-manager to split the cost is reccomended.</p>


    <h2 class="sectionHeading" bind:this={eight}>Section 8 - League Changelog</h2>

    <ul>
        <li> 2025/01/29 - Third place payout was added for $50 (removed the $40 payout that went to the regular season winner to accomodate the change)</li>
    </ul>
</div>
