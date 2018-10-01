Changes a few of the mood effects that affect pawns when the do certain acts, like harvest organs, or eat without a table. 

Changes Listed Below: The first one is original, second is the changes.

Defs\ThoughtDefs\Thoughts_Situation_General.xml


      <li>
        <label>darkness</label>
        <description>I've been in the dark for a while. I don't like it.</description>
        <baseMoodEffect>-5</baseMoodEffect>
        <baseMoodEffect>-3</baseMoodEffect>
      </li>
    </stages>
  </ThoughtDef>

  
  
  
  
Defs\ThoughtDefs\Thoughts_Memory_Social.xml


    <stages>
      <li>
        <label>failed to romance me</label>
        <baseOpinionOffset>-15</baseOpinionOffset>
        <baseOpinionOffset>-5</baseOpinionOffset>
      </li>
    </stages>
  </ThoughtDef>

  
    <durationDays>10</durationDays>
    <durationDays>5</durationDays>  
  
  
Defs\ThoughtDefs\Thoughts_Memory_Death.xml


         <baseMoodEffect>-5</baseMoodEffect>
      </li>
      <li>
        <label>someone organ-harvested</label>
        <label>someone had a vital organ harvested</label>
        <!-- died because of organ harvesting -->
        <description>A prisoner or guest died because the colony took body parts from him. It's horrible.</description>
        <baseMoodEffect>-6</baseMoodEffect>
        <description>A prisoner or guest died because the colony took body parts from him. Maybe they were going to die anyway. </description>
        <baseMoodEffect>-3</baseMoodEffect>
      </li>
    </stages>
  </ThoughtDef>
@ -69,8 +69,8 @@
      <li>
        <label>colonist organ-harvested</label>
        <!-- died because of organ harvesting -->
        <description>A colonist died because someone took body parts from him. It's horrible.</description>
        <baseMoodEffect>-6</baseMoodEffect>
        <description>A colonist died because someone took body parts from him. Maybe they were going to die anyway.</description>
        <baseMoodEffect>-3</baseMoodEffect>
      </li>
    </stages>
  </ThoughtDef>
@ -87,7 +87,7 @@
      <li>
        <label>innocent prisoner died</label>
        <description>One of our prisoners died despite being harmless. We should be able to take care of our prisoners. If we wanted them dead, we could have at least conducted an orderly execution rather than permit that barbarism.</description>
        <baseMoodEffect>-5</baseMoodEffect>
        <baseMoodEffect>-3</baseMoodEffect>
      </li>
    </stages>
  </ThoughtDef>
@ -124,7 +124,7 @@
      <li>
        <label>bonded animal {0} died</label>
        <description>Such a tender, unique animal. This universe is evil!</description>
        <baseMoodEffect>-8</baseMoodEffect>
        <baseMoodEffect>-6</baseMoodEffect>
      </li>
    </stages>
  </ThoughtDef>
  
 --==------========------------===========--------------=================-
 
 Thoughts_Memory_Misc.xml
 
  			<li>
				<label>ate without table</label>
				<description>I had to eat a meal off the ground. Can't we get a table around here?</description>
				<baseMoodEffect>-3</baseMoodEffect>
				<baseMoodEffect>-2</baseMoodEffect>
			</li>
		</stages>
	</ThoughtDef>
@ -109,7 +109,7 @@

	<ThoughtDef>
		<defName>KnowPrisonerSold</defName>
		<durationDays>4</durationDays>
		<durationDays>3</durationDays>
		<stackLimit>5</stackLimit>
		<nullifyingTraits>
			<li>Psychopath</li>
@ -118,14 +118,14 @@
			<li>
				<label>a prisoner was sold</label>
				<description>This colony sold a prisoner into slavery. That's a worrying thought.</description>
				<baseMoodEffect>-3</baseMoodEffect>
				<baseMoodEffect>-2</baseMoodEffect>
			</li>
		</stages>
	</ThoughtDef>

	<ThoughtDef>
		<defName>KnowGuestOrganHarvested</defName>
		<durationDays>8</durationDays>
		<durationDays>6</durationDays>
		<stackLimit>5</stackLimit>
		<stackedEffectMultiplier>0.75</stackedEffectMultiplier>
		<nullifyingTraits>
@ -134,8 +134,8 @@
		<stages>
			<li>
				<label>someone's organ harvested</label>
				<description>The colony took body parts from a guest or prisoner. It's horrible, breaking someone down for parts when they have no choice.</description>
				<baseMoodEffect>-5</baseMoodEffect>
				<description>The colony took body parts from a guest or prisoner. Maybe it was for someone in need.</description>
				<baseMoodEffect>-2</baseMoodEffect>
			</li>
		</stages>
	</ThoughtDef>
@ -172,7 +172,7 @@

	<ThoughtDef>
		<defName>WasImprisoned</defName>
		<durationDays>6</durationDays>
		<durationDays>4</durationDays>
		<stackLimit>1</stackLimit>
		<stages>
			<li>
@ -215,7 +215,7 @@

	<ThoughtDef>
		<defName>KnowBuriedInSarcophagus</defName>
		<durationDays>1</durationDays>
		<durationDays>3</durationDays>
		<stackLimit>10</stackLimit>
		<stages>
			<li>
@ -262,7 +262,7 @@

	<ThoughtDef>
		<defName>KnowButcheredHumanlikeCorpse</defName>
		<durationDays>6</durationDays>
		<durationDays>3</durationDays>
		<stackLimit>1</stackLimit>
		<nullifyingTraits>
			<li>Psychopath</li>
@ -273,7 +273,7 @@
			<li>
				<label>we butchered humanlike</label>
				<description>We butchered someone up like an animal.</description>
				<baseMoodEffect>-6</baseMoodEffect>
				<baseMoodEffect>-2</baseMoodEffect>
			</li>
		</stages>
	</ThoughtDef>
@ -298,7 +298,7 @@
			<li>
				<label>observed corpse</label>
				<description>I saw a dead body laying on the ground. It was disturbing.</description>
				<baseMoodEffect>-4</baseMoodEffect>
				<baseMoodEffect>-2</baseMoodEffect>
			</li>
		</stages>
	</ThoughtDef>
@ -318,7 +318,7 @@
			<li>
				<label>observed rotting corpse</label>
				<description>I saw a rotting corpse laying on the ground. It was disgusting.</description>
				<baseMoodEffect>-6</baseMoodEffect>
				<baseMoodEffect>-4</baseMoodEffect>
			</li>
		</stages>
	</ThoughtDef>
@ -460,7 +460,7 @@
      <li>
        <label>colonist banished</label>
        <description>We just banished someone. I hope they'll make it, but I'm worried.</description>
        <baseMoodEffect>-3</baseMoodEffect>
        <baseMoodEffect>-2</baseMoodEffect>
      </li>
    </stages>
  </ThoughtDef>
@ -477,7 +477,7 @@
      <li>
        <label>colonist banished to death</label>
        <description>We banished someone in such a way that there's almost no way they'll survive.</description>
        <baseMoodEffect>-6</baseMoodEffect>
        <baseMoodEffect>-4</baseMoodEffect>
      </li>
    </stages>
  </ThoughtDef>
@ -494,7 +494,7 @@
      <li>
        <label>prisoner banished to death</label>
        <description>We banished a prisoner in such a way that there's almost no way they'll survive.</description>
        <baseMoodEffect>-4</baseMoodEffect>
        <baseMoodEffect>-2</baseMoodEffect>
      </li>
    </stages>
  </ThoughtDef>
  
  