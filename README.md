<!DOCTYPE html>
<html lang="am">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Harambee University - Wound Care Quiz</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f4f7f6;
            color: #333;
            margin: 0;
            padding: 20px;
        }
        .quiz-container {
            max-width: 800px;
            margin: 0 auto;
            background: #ffffff;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        h1, h2 {
            text-align: center;
            color: #2c3e50;
        }
        .section-title {
            background-color: #e74c3c;
            color: white;
            padding: 10px;
            border-radius: 6px;
            margin-top: 30px;
            font-size: 1.1em;
        }
        .scenario {
            background-color: #f9f9f9;
            border-left: 5px solid #3498db;
            padding: 15px;
            margin: 15px 0;
            font-style: italic;
        }
        .question {
            margin-bottom: 25px;
            padding-bottom: 15px;
            border-bottom: 1px solid #eee;
        }
        .question-text {
            font-weight: bold;
            font-size: 1.05em;
            margin-bottom: 10px;
        }
        .options {
            list-style-type: none;
            padding: 0;
        }
        .option-btn {
            display: block;
            width: 100%;
            text-align: left;
            background: #fff;
            border: 2px solid #bdc3c7;
            padding: 12px;
            margin: 8px 0;
            border-radius: 8px;
            cursor: pointer;
            font-size: 0.95em;
            transition: all 0.2s ease;
        }
        .option-btn:hover {
            background-color: #f0f0f0;
            border-color: #7f8c8d;
        }
        .correct {
            background-color: #2ecc71 !important;
            color: white;
            border-color: #27ae60 !important;
        }
        .incorrect {
            background-color: #e74c3c !important;
            color: white;
            border-color: #c0392b !important;
        }
        .feedback {
            margin-top: 8px;
            font-weight: bold;
            display: none;
        }
        .feedback.correct-text {
            color: #27ae60;
            display: block;
        }
        .feedback.incorrect-text {
            color: #c0392b;
            display: block;
        }
    </style>
</head>
<body>

<div class="quiz-container">
    <h1>Harambee University Department of Nursing</h1>
    <h2>Wound Care Home Take Assignment</h2>
    <hr>

    <!-- GROUP 1 -->
    <div class="section-title">🛑 GROUP 1: DOG BITE AND RABIES MANAGEMENT</div>
    
    <div class="scenario">
        <strong>📍 Scenario 1:</strong> A 14-year-old boy is brought to a health post 30 minutes after being bitten by a stray dog on his right lower leg. The wound is bleeding slightly and there is visible dirt around the area.
    </div>

    <div class="question">
        <div class="question-text">1. What is the first immediate action the nurse should take for this dog bite wound, and why?[span_0](start_span)[span_0](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Apply tight pressure and stitch it immediately to stop bleeding.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Gently cleanse and irrigate the wound to remove dirt and reduce viral/bacterial load.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Cover the wound immediately with a dry sterile dressing without cleaning.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Apply traditional herbs or butter to soothe the skin.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">2. If the dog is suspected to have rabies, within how many hours should anti-rabies treatment ideally be initiated?[span_1](start_span)[span_1](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Within 24 to 48 hours.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">B) Only after the dog shows clear signs of dying.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Within 72 hours.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">D) Immediately/as soon as possible before symptoms develop.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">3. Which specific vaccine must be given to this patient following the dog bite?[span_2](start_span)[span_2](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) BCG Vaccine.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Tetanus Toxoid and Rabies Vaccine (Post-Exposure Prophylaxis).</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Hepatitis B Vaccine.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Oral Polio Vaccine (OPV).</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">4. List two signs that would indicate the wound is becoming infected after a dog bite.[span_3](start_span)[span_3](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, true)">A) Increased pain, redness (erythema), warmth, or purulent drainage (pus).</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">B) Tissue epithelialization and pale pink skin color.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Reduced swelling and formation of a clean scab.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Numbness that disappears within a few minutes.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">5. Why should traditional substances like butter or herbs NOT be applied to this wound?[span_4](start_span)[span_4](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) They keep the wound too dry and cold.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) They introduce debris/bacteria, increase infection risk, and interfere with clinical assessment.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) They neutralize the rabies virus too quickly before the vaccine works.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) They are too expensive to use in rural healthcare settings.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="scenario">
        <strong>📍 Scenario 2:</strong> A 45-year-old farmer was bitten by a rabid dog two days ago but did not seek medical care. He now reports mild headache and anxiety. He asks if rabies affects only the bite area.
    </div>

    <div class="question">
        <div class="question-text">6. Which major body system does rabies primarily affect?[span_5](start_span)[span_5](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Cardiovascular System.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Central Nervous System (CNS).</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Gastrointestinal System.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Musculoskeletal System.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">7. After a dog bite, how soon should medical care ideally be sought, and why?[span_6](start_span)[span_6](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Within a week, because rabies develops very slowly.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Immediately (within hours), to initiate PEP before the virus reaches the nervous system.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Only when the patient starts experiencing hydrophobia.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) After 5 days to observe if the wound heals by primary intention.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">8. Why is it important to report dog bites to a health facility even if the wound looks small?[span_7](start_span)[span_7](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) To ensure the patient pays for hospital insurance.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Because even micro-abrasions can transmit fatal rabies virus and require evaluation/tetanus prophylaxis.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Because small wounds always require extensive surgical debridement.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) To fill out the hospital's statistical annual demographic reports.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <!-- GROUP 2 -->
    <div class="section-title">🛑 GROUP 2: BURN WOUND MANAGEMENT</div>
    
    <div class="scenario">
        <strong>📍 Scenario 3:</strong> A 4-year-old child is rushed to the clinic after spilling hot tea on her chest and upper abdomen. The skin is bright red, blistered, and the child is crying hysterically from severe pain.
    </div>

    <div class="question">
        <div class="question-text">9. Based on the description, what is the depth/degree of this burn wound?[span_8](start_span)[span_8](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Superficial (First-degree) burn.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Partial-thickness (Second-degree) burn.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Full-thickness (Third-degree) burn.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Fourth-degree deep tissue necrosis.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">10. What is the immediate first-aid action for a fresh thermal burn before dressing?[span_9](start_span)[span_9](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Break all the blisters immediately with a clean needle.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">B) Apply ice cubes directly to freeze the tissue.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">C) Cool the burn immediately with clean, cool running tap water for 10-20 minutes.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Coat the area with toothpaste or heavy grease.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">11. Why is fluid resuscitation a priority in extensive burn management?[span_10](start_span)[span_10](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) To wash out the topical ointment from the body.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) To prevent hypovolemic shock due to massive fluid loss from damaged skin barriers.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) To reduce the patient's urge to cry or express pain.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) To accelerate the immediate formation of an eschar.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="scenario">
        <strong>📍 Scenario 4:</strong> An adult patient has deep full-thickness burns covering the entire right arm and the front of the torso. The burned skin looks white, leathery, and charred, and the patient reports surprisingly little pain in the center of the wound.
    </div>

    <div class="question">
        <div class="question-text">12. Why is a full-thickness burn often painless or less painful in the center?[span_11](start_span)[span_11](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) The patient is in psychological denial.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) The heat destroys the local sensory nerve endings in the dermal layer.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) The charred tissue acts as a natural local anesthetic block.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Full-thickness burns do not involve the nerve pathways.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">13. According to the "Rule of Nines", what is the approximate Total Body Surface Area (TBSA) burned?[span_12](start_span)[span_12](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) 9% (Arm only).</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">B) 18% (Front torso only).</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">C) 27% (Right arm 9% + Front torso 18%).</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) 45% (Whole upper body).</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">14. Mention two critical complications a nurse must monitor for in this severe burn patient.[span_13](start_span)[span_13](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Hypertension and excessive skin oiliness.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Hypovolemic shock, systemic infection (sepsis), and compartment syndrome.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Rapid wound healing and skin hyperpigmentation.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) High blood glucose and acute vitamin deficiency.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <!-- GROUP 3 -->
    <div class="section-title">🛑 GROUP 3: SUTURING AND SURGICAL WOUND CARE</div>
    
    <div class="scenario">
        <strong>📍 Scenario 5:</strong> A 25-year-old woman has a clean, linear 4cm laceration on her forearm from a sharp glass edge, occurring 2 hours ago. The nurse prepares to assist with suturing.
    </div>

    <div class="question">
        <div class="question-text">15. By which type of intention will this sutured wound primary heal?[span_14](start_span)[span_14](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, true)">A) Primary Intention.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">B) Secondary Intention.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Tertiary Intention (Delayed Primary).</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Chronic Intention.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">16. What is the main purpose of closing this clean laceration using sutures?[span_15](start_span)[span_15](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) To increase the formation of granulation tissue and slough.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) To approximate the wound edges, minimize scarring, reduce healing time, and prevent infection.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) To allow the wound to remain non-sterile and open to the air.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) To eliminate the need for any post-operative assessment.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">17. Name two sterile items that must be included on the suturing instrument tray.[span_16](start_span)[span_16](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, true)">A) Needle holder, tissue forceps, suture material, and surgical scissors.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">B) Clean unsterile gauze, medical tape, and normal water basin.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Clean gloves, adhesive bandages, and a measuring tape.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Hydrogel dressing, systemic antibiotics, and a permanent marker.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="scenario">
        <strong>📍 Scenario 6:</strong> Five days after a major abdominal surgery, a patient coughs violently. The nurse notes that the surgical incision edges have separated, and loops of bowel are slightly visible.
    </div>

    <div class="question">
        <div class="question-text">18. What is the medical term for the separation of surgical wound layers?[span_17](start_span)[span_17](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Evisceration.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Dehiscence.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Granulation.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Epithelialization.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">19. What is the immediate, critical nursing intervention for an abdominal wound evisceration?[span_18](start_span)[span_18](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Push the organs back into the abdomen immediately using bare hands.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Cover the protruding organs with sterile gauze moistened with sterile normal saline and notify the surgeon immediately.</button>
          
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Leave the wound open to dry out completely under the room fan.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Apply tightly wrapped dry adhesive plaster over the organs.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <!-- GROUP 4 -->
    <div class="section-title">🛑 GROUP 4: WOUND CLEANING AND INFECTION CONTROL</div>
    
    <div class="scenario">
        <strong>📍 Scenario 7:</strong> A nurse is preparing to clean and dress a large, moderately draining pressure ulcer on a patient’s sacrum. The wound bed contains some yellow slough tissue.
    </div>

    <div class="question">
        <div class="question-text">20. What is the preferred, safest standard solution for cleansing clean, granulating wounds?[span_19](start_span)[span_19](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Undiluted Hydrogen Peroxide.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Sterile Normal Saline (0.9% Sodium Chloride) or safe tap water.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Povidone-Iodine surgical scrub.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) 70% Isopropyl Alcohol.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">21. Describe the correct directional technique for cleaning a linear surgical wound?[span_20](start_span)[span_20](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) From the highly contaminated outer perimeter toward the center of the wound.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) From the cleanest area (the incision line) outward to the less clean surrounding skin.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) In a continuous circular motion rubbing back and forth rapidly.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) From the bottom of the dressing up to the top skin edge.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">22. What type of dressing is indicated for a wound that requires mechanical debridement of non-viable tissue?[span_21](start_span)[span_21](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Dry-to-dry sterile dressing.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Wet-to-dry dressing technique.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Impermeable plastic wrap.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Thin transparent adhesive tape only.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="scenario">
        <strong>📍 Scenario 8:</strong> A patient’s post-operative wound has become increasingly painful, swollen, and red. The dressing is soaked with thick, foul-smelling, yellowish-green drainage.
    </div>

    <div class="question">
        <div class="question-text">23. What type of wound drainage is described as thick, cloudy, and varying in color (yellow/green/brown)?[span_22](start_span)[span_22](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Serous exudate.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">B) Sanguineous exudate.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Serosanguineous exudate.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Purulent exudate.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">24. Which clinical procedure should the nurse perform to identify the specific bacteria causing this infection?[span_23](start_span)[span_23](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, true)">A) Take an automated wound swab for culture and sensitivity testing.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">B) Measure the length and depth of the wound with a ruler.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Apply an extra layer of dry gauze.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Perform sharp mechanical debridement under running water.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <!-- GROUP 5 -->
    <div class="section-title">🛑 GROUP 5: HEALING PROCESS AND PATIENT FACTORS</div>
    
    <div class="scenario">
        <strong>📍 Scenario 9:</strong> A 60-year-old patient with diabetes mellitus and a 20-year smoking history has a slow-healing foot ulcer. The nurse reviews factors affecting wound healing.
    </div>

    <div class="question">
        <div class="question-text">25. How does diabetes mellitus delay the wound healing process?[span_24](start_span)[span_24](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) It causes excessive tissue oxygenation and rapid blood flow.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) It impairs leukocyte function, compromises microvascular circulation, and delays collagen synthesis.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) It speeds up the inflammatory phase too quickly.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) It converts chronic wounds into acute primary intention wounds.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">26. How does nicotine/smoking interfere with tissue repair?[span_25](start_span)[span_25](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) It acts as a vasodilator increasing local blood supply.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) It causes vasoconstriction, reduces oxygen-carrying capacity (carboxyhemoglobin), and leads to tissue hypoxia.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) It increases the production of red blood cells in the wound.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) It keeps the wound bed excessively moist.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">27. During the inflammatory phase of healing, what four local signs are expected around a wound?[span_26](start_span)[span_26](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Scarring, blanching, numbness, and cooling.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Redness (rubor), heat (calor), swelling (tumor), and pain (dolor).</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Desiccation, maceration, undermining, and tunneling.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Granulation, epithelialization, remodeling, and maturation.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">28. Which cells play the major role in phagocytosis and fighting infection during the inflammatory phase?[span_27](start_span)[span_27](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Erythrocytes and platelets.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Leukocytes (Neutrophils and Macrophages).</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Fibroblasts and endothelial cells.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Keratinocytes and melanocytes.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">29. The proliferative phase of healing involves the formation of which two key structures?[span_28](start_span)[span_28](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) Thick white eschar and dry scabs.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) Granulation tissue and new blood vessels (angiogenesis).</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) Deep sensory nerves and skeletal muscle fibers.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) Surgical sutures and medical staples.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="scenario">
        <strong>📍 Scenario 10:</strong> A post-operative patient is not eating well, has poor fluid intake, and refuses to mobilize. The nurse observes that the surgical wound is healing very slowly.
    </div>

    <div class="question">
        <div class="question-text">30. How does poor nutrition (specifically protein and Vitamin C deficiency) affect wound healing?[span_29](start_span)[span_29](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) It prevents the wound from producing foul odors.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) It impairs collagen synthesis, delays tissue granulation, and weakens anatomical tensile strength.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) It accelerates the maturation and remodeling phase.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) It reduces the risk of dehiscence or evisceration.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">31. What is the primary goal of wound dressing application in clinical nursing?[span_30](start_span)[span_30](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) To permanently hide the wound from the patient's family sight.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) To maintain a clean/moist environment, protect from microbes, absorb excess exudate, and promote healing.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) To ensure the wound dries out completely into a hard crust.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) To avoid documenting the wound's physical characteristics.</button>
        </div>
        <div class="feedback"></div>
    </div>

    <div class="question">
        <div class="question-text">32. Why must all dressing materials remain completely sterile before use?[span_31](start_span)[span_31](end_span)</div>
        <div class="options">
            <button class="option-btn" onclick="checkAnswer(this, false)">A) To keep the dressing from sticking to the medical tape.</button>
            <button class="option-btn" onclick="checkAnswer(this, true)">B) To prevent introducing exogenous pathogens into the wound, reducing infection risk.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">C) To minimize the financial cost of hospital materials.</button>
            <button class="option-btn" onclick="checkAnswer(this, false)">D) To maintain the patient's core body temperature.</button>
        </div>
        <div class="feedback"></div>
    </div>

</div>

<script>
    function checkAnswer(button, isCorrect) {
        // ማሰሻውን (options container) ማግኘት
        const optionsContainer = button.parentElement;
        const buttons = optionsContainer.getElementsByClassName('option-btn');
        const feedbackDiv = optionsContainer.nextElementSibling;

        // ሁሉንም በተኖች ማዘጋት (ተማሪው ደግሞ ደጋግሞ እንዳይነካ)
        for (let btn of buttons) {
            btn.disabled = true;
        }

        // ልክ ከሆነ አረንጓዴ፣ ስህተት ከሆነ ቀይ ማሳያ
        if (isCorrect) {
            button.classList.add('correct');
            feedbackDiv.textContent = "✅ ትክክለኛ መልስ!";
            feedbackDiv.className = "feedback correct-text";
        } else {
            button.classList.add('incorrect');
            feedbackDiv.textContent = "❌ ስህተት ነው! ትክክለኛውን መልስ ከላይ በ'የመልስ ቁልፍ' ላይ ያረጋግጡ።";
            feedbackDiv.className = "feedback incorrect-text";
            
            // እውነተኛውን መልስ ለአገዝና አረንጓዴ ማድረግ
            for (let btn of buttons) {
                if (btn.getAttribute('onclick').includes('true')) {
                    btn.classList.add('correct');
                }
            }
        }
    }
</script>

</body>
</html>
            
