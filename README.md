# The-junk-food-secrets
How america is poisoning the future of our nation what is really in our food
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fuel Station | Junk Food Decoder</title>
    <style>
        body { font-family: sans-serif; background-color: #1a1a1a; color: white; padding: 20px; }
        h1 { color: #ccff00; text-align: center; }
        .search-container { text-align: center; margin-bottom: 20px; }
        #searchInput {
            padding: 12px;
            width: 80%;
            max-width: 400px;
            border-radius: 25px;
            border: none;
            font-size: 16px;
        }
        table { width: 100%; border-collapse: collapse; background: #2a2a2a; margin-top: 10px; }
        th, td { padding: 12px; text-align: left; border-bottom: 1px solid #444; }
        th { background-color: #333; color: #ccff00; position: sticky; top: 0; }
        tr:hover { background-color: #3a3a3a; }
        .red-flag { color: #ff4444; font-weight: bold; }
        .food-name { color: #ccff00; font-weight: bold; }
    </style>
</head>
<body>

    <h1>Junk Food Decoder</h1>
    <div class="search-container">
        <input type="text" id="searchInput" onkeyup="filterTable()" placeholder="Search for a food or ingredient...">
    </div>

    <table id="foodTable">
        <thead>
            <tr>
                <th>#</th>
                <th>Food Item</th>
                <th>Main Ingredients</th>
                <th>The Red Flag</th>
            </tr>
        </thead>
        <tbody>
            <tr><td>1</td><td class="food-name">Snickers</td><td>Milk chocolate, peanuts, corn syrup, sugar</td><td class="red-flag">High fructose corn syrup & trans fats.</td></tr>
            <tr><td>2</td><td class="food-name">Doritos (Nacho Cheese)</td><td>Corn, vegetable oil, MSG, Red 40, Yellow 5</td><td class="red-flag">MSG triggers overeating; artificial dyes.</td></tr>
            <tr><td>3</td><td class="food-name">Oreos</td><td>Enriched flour, sugar, palm oil, high fructose corn syrup</td><td class="red-flag">Zero fiber; high "shelf-stable" fats.</td></tr>
            <tr><td>4</td><td class="food-name">Cheetos (Crunchy)</td><td>Enriched corn meal, vegetable oil, cheese seasoning</td><td class="red-flag">High sodium and Yellow 6 dye.</td></tr>
            <tr><td>5</td><td class="food-name">Twinkies</td><td>Enriched wheat flour, sugar, corn syrup, beef fat</td><td class="red-flag">High calorie density; uses tallow (beef fat).</td></tr>
            <tr><td>6</td><td class="food-name">Skittles</td><td>Sugar, corn syrup, hydrogenated palm kernel oil</td><td class="red-flag">Mostly sugar and Titanium Dioxide.</td></tr>
            <tr><td>7</td><td class="food-name">Lays Classic Chips</td><td>Potatoes, vegetable oil, salt</td><td class="red-flag">High acrylamide (byproduct of frying).</td></tr>
            <tr><td>8</td><td class="food-name">Pop-Tarts (Strawberry)</td><td>Corn syrup, high fructose corn syrup, enriched flour</td><td class="red-flag">Double daily sugar in one pack.</td></tr>
            <tr><td>9</td><td class="food-name">Reese’s Cups</td><td>Milk chocolate, peanuts, sugar, dextrose</td><td class="red-flag">Dextrose spikes blood sugar instantly.</td></tr>
            <tr><td>10</td><td class="food-name">Sour Patch Kids</td><td>Sugar, invert sugar, corn syrup, tartaric acid</td><td class="red-flag">High acidity; destroys tooth enamel.</td></tr>
            <tr><td>11</td><td class="food-name">Pringles</td><td>Dried potatoes, vegetable oil, rice flour, wheat starch</td><td class="red-flag">High in "refined" starches, not potato slices.</td></tr>
            <tr><td>12</td><td class="food-name">Kit Kat</td><td>Sugar, wheat flour, cocoa butter, palm kernel oil</td><td class="red-flag">High saturated fat from palm oil.</td></tr>
            <tr><td>13</td><td class="food-name">Gummy Bears</td><td>Corn syrup, sugar, gelatin, citric acid</td><td class="red-flag">Pure sugar with animal-based gelatin.</td></tr>
            <tr><td>14</td><td class="food-name">M&Ms (Milk)</td><td>Milk chocolate, sugar, cornstarch, Blue 1 & 2</td><td class="red-flag">Heavy use of artificial food colorings.</td></tr>
            <tr><td>15</td><td class="food-name">Hot Pockets</td><td>Enriched flour, water, imitation cheese, meat</td><td class="red-flag">High in nitrates and "imitation" fillers.</td></tr>
            <tr><td>16</td><td class="food-name">Cosmic Brownies</td><td>Enriched flour, palm oil, corn syrup, cocoa</td><td class="red-flag">Contains "TBHQ" (a preservative).</td></tr>
            <tr><td>17</td><td class="food-name">Goldfish Crackers</td><td>Enriched wheat flour, cheddar cheese, vegetable oils</td><td class="red-flag">High refined carbs; autolyzed yeast.</td></tr>
            <tr><td>18</td><td class="food-name">Starburst</td><td>Sugar, corn syrup, hydrogenated palm kernel oil</td><td class="red-flag">Sticks to teeth, increasing cavity risk.</td></tr>
            <tr><td>19</td><td class="food-name">Beef Jerky</td><td>Beef, sugar, soy sauce, sodium nitrite</td><td class="red-flag">Extremely high sodium and nitrites.</td></tr>
            <tr><td>20</td><td class="food-name">Twix</td><td>Milk chocolate, enriched flour, sugar, palm oil</td><td class="red-flag">High ratio of biscuit-to-caramel sugar.</td></tr>
            <tr><td>21</td><td class="food-name">Ritz Crackers</td><td>Enriched flour, palm oil, sugar, HFCS</td><td class="red-flag">Surprisingly high in sugar for a salty snack.</td></tr>
            <tr><td>22</td><td class="food-name">Cheez-Its</td><td>Enriched flour, vegetable oil, skim milk cheese</td><td class="red-flag">High in saturated fats and refined flour.</td></tr>
            <tr><td>23</td><td class="food-name">Mountain Dew</td><td>Water, HFCS, citric acid, Yellow 5</td><td class="red-flag">Massive sugar load + artificial dye.</td></tr>
            <tr><td>24</td><td class="food-name">Hostess Cupcakes</td><td>Sugar, water, enriched flour, corn syrup</td><td class="red-flag">Multiple types of sugar in one serving.</td></tr>
            <tr><td>25</td><td class="food-name">Slim Jims</td><td>Beef, pork, chicken, salt, sodium nitrite</td><td class="red-flag">Highly processed "separated" meats.</td></tr>
            <tr><td>26</td><td class="food-name">Tostitos</td><td>Corn, vegetable oil, salt</td><td class="red-flag">High calorie count with very little fullness.</td></tr>
            <tr><td>27</td><td class="food-name">Rice Krispies Treats</td><td>Rice cereal, corn syrup, fructose, margarine</td><td class="red-flag">Low calorie but almost 100% simple carbs.</td></tr>
            <tr><td>28</td><td class="food-name">Fruit Roll-Ups</td><td>Corn syrup, sugar, pear puree</td><td class="red-flag">Mostly corn syrup, very little real fruit.</td></tr>
            <tr><td>29</td><td class="food-name">Fritos</td><td>Corn, corn oil, salt</td><td class="red-flag">One of the highest fat-to-corn ratios.</td></tr>
            <tr><td>30</td><td class="food-name">Ding Dongs</td><td>Sugar, water, enriched flour, palm oil</td><td class="red-flag">High in artificial vanillin and fats.</td></tr>
            <tr><td>31</td><td class="food-name">Butterfinger</td><td>Corn syrup, sugar, peanuts, vegetable oil</td><td class="red-flag">High in hydrogenated oils (bad for heart).</td></tr>
            <tr><td>32</td><td class="food-name">Combos</td><td>Enriched wheat flour, vegetable oil, dairy wheys</td><td class="red-flag">Filling is mostly oils and food starches.</td></tr>
            <tr><td>33</td><td class="food-name">Milky Way</td><td>Milk chocolate, sugar, corn syrup, palm oil</td><td class="red-flag">High glycemic index (causes crashes).</td></tr>
            <tr><td>34</td><td class="food-name">Funyuns</td><td>Enriched corn meal, onion powder, MSG</td><td class="red-flag">No actual onions; mostly corn and flavor.</td></tr>
            <tr><td>35</td><td class="food-name">Chips Ahoy!</td><td>Enriched flour, chocolate chips, sugar, palm oil</td><td class="red-flag">High in soy lecithin and artificial flavors.</td></tr>
            <tr><td>36</td><td class="food-name">Nutter Butter</td><td>Enriched flour, sugar, peanut butter, palm oil</td><td class="red-flag">Uses partially hydrogenated oils.</td></tr>
            <tr><td>37</td><td class="food-name">Pretzels</td><td>Enriched flour, salt, corn syrup, canola oil</td><td class="red-flag">White flour spikes insulin quickly.</td></tr>
            <tr><td>38</td><td class="food-name">Donuts (Glazed)</td><td>Enriched flour, sugar, water, shortening</td><td class="red-flag">Fried in oil and dipped in sugar.</td></tr>
            <tr><td>39</td><td class="food-name">Cup Noodles</td><td>Enriched flour, palm oil, salt, MSG</td><td class="red-flag">One cup has ~50% of your daily salt.</td></tr>
            <tr><td>40</td><td class="food-name">Beef Ravioli</td><td>Tomatoes, water, enriched flour, beef</td><td class="red-flag">High in sugar and textured vegetable protein.</td></tr>
            <tr><td>41</td><td class="food-name">Bugles</td><td>Corn meal, coconut oil, sugar</td><td class="red-flag">Very high saturated fat from coconut oil.</td></tr>
            <tr><td>42</td><td class="food-name">Fruit Gushers</td><td>Sugar, corn syrup, pear puree</td><td class="red-flag">High modified corn starch content.</td></tr>
            <tr><td>43</td><td class="food-name">3 Musketeers</td><td>Milk chocolate, sugar, corn syrup, palm oil</td><td class="red-flag">Nougat is almost entirely whipped sugar.</td></tr>
            <tr><td>44</td><td class="food-name">Ho Hos</td><td>Sugar, enriched flour, palm kernel oil</td><td class="red-flag">High in polysorbate 60 (emulsifier).</td></tr>
            <tr><td>45</td><td class="food-name">Wheat Thins</td><td>Enriched flour, sugar, soybean oil, salt</td><td class="red-flag">Sugar is the 2nd or 3rd ingredient.</td></tr>
            <tr><td>46</td><td class="food-name">Lucky Charms</td><td>Whole grain oats, sugar, marshmallows</td><td class="red-flag">Marshmallows are gelatin and sugar.</td></tr>
            <tr><td>47</td><td class="food-name">Nilla Wafers</td><td>Enriched flour, sugar, HFCS</td><td class="red-flag">Pure simple sugar and refined flour.</td></tr>
            <tr><td>48</td><td class="food-name">Famous Amos</td><td>Enriched flour, chocolate chips, sugar, palm oil</td><td class="red-flag">High calorie density in small portions.</td></tr>
            <tr><td>49</td><td class="food-name">Takis Fuego</td><td>Corn masa, vegetable oil, seasoning, Red 40</td><td class="red-flag">Extreme spice/acidity (harsh on stomach).</td></tr>
            <tr><td>50</td><td class="food-name">Honey Buns</td><td>Enriched flour, sugar, shortening</td><td class="red-flag">Over 500 calories in one single bun.</td></tr>
        </tbody>
    </table>

    <script>
        function filterTable() {
            var input, filter, table, tr, td, i, txtValue;
            input = document.getElementById("searchInput");
            filter = input.value.toUpperCase();
            table = document.getElementById("foodTable");
            tr = table.getElementsByTagName("tr");

            for (i = 1; i < tr.length; i++) {
                tr[i].style.display = "none";
                td = tr[i].getElementsByTagName("td");
                for (var j = 0; j < td.length; j++) {
                    if (td[j]) {
                        txtValue = td[j].textContent || td[j].innerText;
                        if (txtValue.toUpperCase().indexOf(filter) > -1) {
                            tr[i].style.display = "";
                            break;
                        }
                    }
                }
            }
        }
    </script>

</body>
</html>
