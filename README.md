# choco-dist
    public:
    long long findMinDiff(vector<long long> a, long long n, long long m){
    //code
         sort(a.begin(),a.end());
         int min_diff=INT_MAX;
         int diff=0;
         for(int i=0;i+m-1<n;i++){
             diff=a[i+m-1]-a[i];
             if(diff<min_diff)
             {
                 min_diff=diff;
             }
         }
         return min_diff;
    }
};
