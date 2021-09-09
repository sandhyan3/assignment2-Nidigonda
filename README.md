# assignment2-nidigonda

# Nidigonda Sandhya

###### Jammu and kashmir

Popularly known as the "Paradise on Earth", Jammu and Kashmir is world famous for its scenic splendour, **snow-capped mountains**, plentiful wildlife, **exquisite monuments**, hospitable people and local handicrafts.I like Jammu and kashmir
because of its pleaseant environment and Mountains and its one of my favourite trip  with my family.
---
# Directions to favorite place with ordered list and unordered list. 
 
 1. Maryville
 2. Kansas city 
 3. Chicago 
 4. India
    1. Jammu and Kashmir airport 
    2. Gulmarg
    3. pahalgam
    4. sonmarg 
 5. Srinagar city
 
 * Items to carry
   * Pack warm cloths
   * Carry cold cream
   * Warm socks
   * overcoats
 * To Board the flight 
   * Carry Identity Proof 
   * Carry sufficient cash

   **[click hear for AboutME](AboutMe.md)**

   ---
# Foods to try
  
   Below is the list of food and drinks one must try.

   | Food/Drinks | Location | Price |
   | ----- | ----- | ----- |
   | kitkat milkshake | Hyderabad | 80 |
   | Cobb salad | Maryville | 100 |
   | Briyani | Hyderabad | 120 |
   | coke | Mumbai | 60 |

   ---
# Quotes
   > "Your time is limited, so don't waste it living someone else's life. Don't be trapped by dogma – which is living with the results of other people's thinking.- *Steve Jobs*

   > "If you set your goals ridiculously high and it's a failure, you will fail above everyone else's success. -*James Cameron*

   ---
# Games on arbitrary graphs
 
 Let a game be played by two players on an arbitrary graph G. I.e. the current state of the game is a certain vertex. The players perform moves by turns, and move from the current vertex to an adjacent vertex using a connecting edge. Depending on the game, the person that is unable to move will either lose or win the game.
 
 vector<vector<int>> adj_rev;

vector<bool> winning;
vector<bool> losing;
vector<bool> visited;
vector<int> degree;

void dfs(int v) {
    visited[v] = true;
    for (int u : adj_rev[v]) {
        if (!visited[u]) {
            if (losing[v])
                winning[u] = true;
            else if (--degree[u] == 0)
                losing[u] = true;
            else
                continue;
            dfs(u);
        }
    }
}

[click for Games on arbitrary graphs](https://cp-algorithms.com/game_theory/games_on_graphs.html)




