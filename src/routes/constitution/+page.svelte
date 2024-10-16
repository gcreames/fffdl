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
    <h1 class="noUnderscore">LEGENDS LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(one)}>Section 1: Roster</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneOne)}>1.1 Positional Breakdown</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneTwo)}>1.2 Trading & Drafts</h4>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoOne)}>1.2.1 Initial Draft</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoTwo)}>1.2.2 Rookie Drafts</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoThree)}>1.2.3 Trade Deadline</h5>
            <h5 class="noUnderscore clickable" on:click={() => goToSection(oneTwoFour)}>1.2.4 Trade Restrictions</h5>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(oneThree)}>1.3 Waiver Wire</h4>
    
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(two)}>Section 2: Scoring System</h3>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(three)}>Section 3: Payment</h3>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(four)}>Section 4: Postseason</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourOne)}>4.1 Playoffs</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fourTwo)}>4.2 Playoff Tiebreakers</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(five)}>Section 5: Tanking Policy</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(fiveOne)}>5.1 League Tanking Policy</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(six)}>Section 6: League Median</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sixOne)}>6.1 League Median</h4>

    <h3 class="noUnderscore clickable" on:click={() => goToSection(seven)}>Section 7: Division/Schedule</h3>
    
        <h4 class="noUnderscore clickable" on:click={() => goToSection(sevenOne)}>7.1 Division/Schedule</h4>
    
    
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1 Roster Breakdown</h2>
    
    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 Positional Breakdown</h3>
    
    <p>28 Total Players</p>
    
    <p class="underscore">Starters</p>
    <ul>
        <li>QB</li>
        <li>RB</li>
        <li>RB</li>
        <li>WR</li>
        <li>WR</li>
        <li>WR</li>
        <li>TE</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>SUPERFLEX (QB/RB/WR/TE</li>
    </ul>
    
    <p>18 Bench (Not including Taxi-Squad or Injury Reserve)</p>

    <p>4 Taxi-Squad (Roster sports for rookies/sophomores to be stashed without taking up one of your 28 actual roster spots; once a player is added to the taxi-squad and moved to the active roster, they can not be placed back onto the Taxi-Squad until after the season is over)</p>

    <p>1 IR Spots (Player must be labeled as IR, PUP, or Out in the Sleeper App)</p>
    


    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 Trading & Drafts</h3>
    
    <p>Trading of players and draft picks (up to 3 drafts away) are allowed. Trades will be processed immediately. Tradable assets include players, draft picks, and FAAB $.</p>
    
    <h4 bind:this={oneTwoOne}>1.2.1 Initial Draft</h4>
    <div class="subBlock">
        <p>First draft will be derby style (Lottery for pick selection order; ex: If I get 1st in the draft lottery, I get to pick which pick I want for the snake draft, 2nd pick gets the next selection of what draft position they want, and so on. The 12th pick in the lottery gets the remaining pick that nobody else chose). This draft will be highly important as the waiver wire will be slim and obviously these guys will be on your team every year. 24 rounds.</p>

    </div>

    <h4 bind:this={oneTwoTwo}>1.2.2 Rookie Draft</h4>
    <div class="subBlock">
        <p>First draft will be derby style (Lottery for pick selection order; ex: If I get 1st in the draft lottery, I get to pick which pick I want for the snake draft, 2nd pick gets the next selection of what draft position they want, and so on. The 12th pick in the lottery gets the remaining pick that nobody else chose). This draft will be highly important as the waiver wire will be slim and obviously these guys will be on your team every year. 24 rounds.</p>
    </div>
    
    <h4 bind:this={oneTwoThree}>1.2.3 Trade Deadline</h4>
    <div class="subBlock">
        <p>The trade deadline will be set for Week 14 of the NFL season.</p>
    </div>
    
    <h4 bind:this={oneTwoFour}>1.2.4 Trade Restrictions</h4>
    <div class="subBlock">
        <p>You will not be able to trade draft picks that are more than 3 drafts away. For example, during the 2021 season, you cannot trade any picks in or after the 2025 draft. You may only trade FAAB $ from the current season.</p>
    </div>
    
    
    
    <h3 bind:this={oneThree}>1.3 Waiver Wire</h3>
    
    <p>Auction system; $100 FAAB (free agent auction bidding) to each player for the season, bid on players each week; waivers open on Wednesdays after the week has concluded; tiebreaker on a bid goes to inverted standings; Waivers will be scarce with the number of guys on each team, so this shouldn’t be a big aspect of the league..</p>

    <p>FAAB budgets will reset each season.</p>

    
    <h2 class="sectionHeading" bind:this={two}>Section 2 Scoring System</h2>

    <h3 bind:this={twoOne}>2.1 Scoring System</h3>
    <p>ESPN standard PPR with exception to TE PPR Premium (TE receives 1.5 PPR to bring more value to the position)</p>

    <h2 class="sectionHeading" bind:this={three}>Section 3 Payment</h2>
    <p>$50 per year entry fee; $50 pre-payment for following season to reduce people exiting the league with no penalty; if you leave (Most likely because your team sucks), your entry fee will be given to the individual who takes over your (most likely) garbage team to incentivize them to take your place. This may sound like it sucks but it’s the only way to make sure people take it seriously and want to keep this thing going for a while.

Payout Structure: $350 to 1st, $150 to 2nd, $50 to 3rd, and $50 to Reg Szn Champ; top 3 of 12 at least make money back.</p>
    
    <h2 class="sectionHeading" bind:this={four}>Section 4 Postseason</h2>
    
    <h3 bind:this={fourOne}>4.1 Playoffs</h3>
    <p>At the end of the season 8 teams will make the playoffs. Top 8 records. Higher seeds get to pick who their opponent is for “Home field advantage” in the first round; start with the 1 seed, then 2, then 3, and 4th will be automatically decided; this way top 3 teams get an advantage without it being raw point</p>
    
    <h3 bind:this={fourTwo}>4.2 Seeding Tiebreakers</h3>
    <p>If two teams finish with the same record the tiebreakers will go as followed:</p>

    <ol>
        <li>Head 2 Head Record</li>
        <li>Most Points Scored</li>
        <li>Most Points Against</li>
        <li>Coin Flip</li>
    </ol>

    <h2 class="sectionHeading" bind:this={five}>Section 5 Tanking Policy</h2>
    
    <h3 bind:this={fiveOne}>5.1 League Tanking Policy</h3>
    <p>No team may intentionally leave starting roster spots empty. Any evidence of intentionally leaving roster spots empty in order to improve your draft position may be subject to punishment, including but not limited to the forfeiture of draft selections.</p>

    <h2 class="sectionHeading" bind:this={six}>Section 6 League Median</h2>
    
    <h3 bind:this={sixOne}>6.1 League Median</h3>
    <p>Extra game league median record style; this means you play head-to-head for a W/L but also the top 6 scoring teams each week receive an extra win while the bottom 6 receive a loss, this would make records out of 28 rather than 14.</p>

    <h2 class="sectionHeading" bind:this={seven}>Section 7 Division/Schedule</h2>
    
    <h3 bind:this={sevenOne}>7.1 Division/Schedule</h3>
    <p>1 large division; everybody plays everybody else 1 time with two extra games; Playoffs start in week 15 and go to week 17 to hopefully avoid guys sitting out the last week of the season.</p>
    

</div>
