
#include <bits/stdc++.h>

using namespace std;

using ll = long long;
using vi = vector<int>;
using vvi = vector<vector<int>>;
using vl = vector<ll>;
using vvl = vector<vector<ll>>;
using pi = pair<int, int>;
using pl = pair<ll, ll>;


#define all(x) begin(x), end(x)
#define rall(x) rbegin(x), rend(x)
#define pb push_back
#define mp make_pair
#define f first
#define s second
#define endl '\n'
#define forn(i, n) for(ll i = 0; i < n; i++)
#define fora(i, a, n) for(ll i = a; i < n; i++)
#define readi(e) int e; cin >> e
#define readl(e) ll e; cin >> e
#define reads(e) string e; cin >> e
#define t int tt; cin >> tt; while(tt--)


template<typename U>
void print(U arr) {
	for(auto element: arr) {
		cout << element << " ";
	}
	cout << endl;
}
const int MAX_N = 1e9+7;
//DFS
/*
int n, m, vis[MAX_N];
vector<int> adj[MAX_N];

void dfs(int u) {
    vis[u] = 1;
    for (int v : adj[u]) {
        if (vis[v]) continue;
        dfs(v);
    }
}

void solve() {
    cin >> n >> m;
    for (int i = 0; i < m; i++) {
        int u, v; cin >> u >> v;
        adj[u].push_back(v);
        adj[v].push_back(u);
    }
    for (int i = 1; i <= n; i++) {
        if (vis[i]) continue;
        dfs(i);
    }
}  */
// BFS
/*
int n, m;
vector<int> adj[MAX_N], dist;

void bfs(int s) {
    dist.assign(n + 1, -1);
    queue<int> q;
    dist[s] = 0; q.push(s);
    while (q.size()) {
        int u = q.front(); q.pop();
        for (int v : adj[u]) {
            if (dist[v] == -1) {
                dist[v] = dist[u] + 1;
                q.push(v);
            }
        }
    }
}

void solve() {
    cin >> n >> m;
    for (int i = 0; i < m; i++) {
        int u, v; cin >> u >> v;
        adj[u].push_back(v);
        adj[v].push_back(u);
    }
    bfs(1);
}
 */
 
 // bipartite coloring
 /*
 int n, m, color[MAX_N];
vector<int> adj[MAX_N];

void bfs(int s) {
    queue<int> q;
    color[s] = 1; q.push(s);
    while (q.size()) {
        int u = q.front(); q.pop();
        for (int v : adj[u]) {
            if (!color[v]) {
                color[v] = color[u] % 2 + 1;
                q.push(v);
            }
            else if (color[v] == color[u]) {
                cout << "IMPOSSIBLE\n";
                exit(0);
            }
        }
    }
}

void solve() {
    cin >> n >> m;
    for (int i = 0; i < m; i++) {
        int u, v; cin >> u >> v;
        adj[u].push_back(v);
        adj[v].push_back(u);
    }
    for (int i = 1; i <= n; i++)
        if (!color[i])
            bfs(i);
    for (int i = 1; i <= n; i++) 
        cout << color[i] << " ";
    cout << "\n";
}
*/
// read and write into files, rather than standard i/o
void setup(string s) {
	freopen((s+".in").c_str(), "r", stdin);
	freopen((s+".out").c_str(), "w", stdout);
}


void fun(){











}

int main(void) {
	ios::sync_with_stdio(false);
	cin.tie(0);

fun();

	return 0;
}
