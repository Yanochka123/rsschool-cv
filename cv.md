# cv
## Norkina Yaroslava
*Contacts*: diskord norikin_yaroslava; telegram @fvfngrdth; janorka2004@gmail.com

![Here I am](/IMG_20230624_155904.jpg)

## About me
I am studying at ITMO University with a degree in Mobile and Network Technologies and want to become a front-end developer. I would like to learn a relevant and interesting profession, so in my free time from studying, I decided to take courses from rsschool. My goal is to become a good specialist and within six months to gain the work skills necessary for employment. At the moment, I participated in team educational projects, where I tried myself as a developer: a photo conversion site and a university job search site “ITMO-HUNTER”. I am extremely inspired by the result, but I still lack skills in website layout and design

**I have skills in working with Git, figma, photoshop, program in C++, python, html&css, use vs code and pycharm, have used Docker, Linux VM**

Code example

'''
#include <algorithm>
#include <iostream>
#include <vector>
using namespace std;

bool has_cycle = false;
'''

'''
void dfs(const int& v, const vector<vector<int>>& edges, vector<int>& colors, vector<int>& path) {
    if (has_cycle) return;

    colors[v] = 1;
    path.push_back(v + 1);
    for (const int& u : edges[v]) {
        if (colors[u] == 0) {
            dfs(u, edges, colors, path);
        } else if (colors[u] == 1) {
            path.push_back(u + 1);
            has_cycle = true;
            return;
        }
        if (has_cycle) return;
    }
    colors[v] = 2;
    path.pop_back();
}
'''

'''
int main() {
    int n, m;
    cin >> n >> m;
    vector<vector<int>> edges(n);
    for (int i = 0; i < m; i++) {
        int u, v;
        cin >> u >> v;
        --u, --v;
        edges[u].push_back(v);
    }
    vector<int> colors(n, 0);
    vector<int> path;
    for (int v = 0; v < n; v++) {
        if (colors[v] == 0) {
            dfs(v, edges, colors, path);
            if (has_cycle) {
                break;
            }
        }
    }
    if (!has_cycle) {
        cout << "NO\n";
    } else {
        cout << "YES" << endl;
        auto it = path.end() - 2;
        for (; *it != path.back(); it--) {} //ищем вершину в которой зациклились

        for (;it != path.end() - 1; it++) { //выводим
            cout << *it << " ";
        }
        cout << endl;
    }
    return 0;
}
'''

## Work experience 
Participation in training projects and team interaction

[image-to-sketch](https://github.com/KERILL-I/image-to-sketch), [itmo-hunter](https://github.com/MKYrii/programming_project.git)

### Place of study - ITMO University
### English language intermediate level
