int lengthOfLongestAP(int ar[], int n) {
        unordered_map<int,int> mp;
        for(int i=0;i<n;i++)
            mp[ar[i]]=1;
        int mxlen=1;
        for(int i=0;i<n;i++)
        {
            for(int j=i+1;j<n;j++)
            {
                int pre=ar[i];
                int cur=ar[j];
                int diff=cur-pre;
                int cnt=1;
                while(cur<=ar[n-1] && mp.find(cur)!=mp.end())
                {
                    cur+=diff;
                    cnt++;
                }
                mxlen=max(cnt,mxlen);
            }
        }
        return mxlen;
    }
