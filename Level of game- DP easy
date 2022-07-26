//Initial Template for C++

#include <bits/stdc++.h>
using namespace std;

// } Driver Code Ends
//User function Template for C++

class Solution{
    public:
        int dp[1001][1001];
        int game_score(int h, int m){
            if(h<=0 ||m<=0) return 0;
            
            if(dp[h][m] != -1) return dp[h][m];
            
            int firstsec = game_score(h-2,m-8)+2;
            int firstthird = game_score(h-17,m+7)+2;
            
            return dp[h][m] = max(firstsec,firstthird);
        }
        int maxLevel(int h,int m)
        {
            memset(dp,-1,sizeof(dp));
            return game_score(h,m) -1;
        }
};

//{ Driver Code Starts.

int main()
{
    int t;
    cin>>t;
    Solution a;
    while(t--)
    {
        int h,m;
        cin>>h>>m;
        cout<<a.maxLevel(h,m)<<endl;
    }
    return 0;
}
// } Driver Code Ends
