class Solution {
public:
    vector<string> ans;

    void solve(string s, int idx) {
        if (idx == s.size()) {
            ans.push_back(s);
            return;
        }

        if (isdigit(s[idx])) {
            solve(s, idx + 1);
        } else {
            s[idx] = tolower(s[idx]);
            solve(s, idx + 1);

            s[idx] = toupper(s[idx]);
            solve(s, idx + 1);
        }
    }

    vector<string> letterCasePermutation(string s) {
        solve(s, 0);
        return ans;
    }
};
