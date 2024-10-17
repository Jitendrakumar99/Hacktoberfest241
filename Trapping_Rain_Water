// leetcode question
int trap(vector<int>& height) {
        int n=height.size();
        int lefth[n];
        int righth[n];
        lefth[0]=height[0];
        righth[n-1]=height[n-1];
        for(int i=1;i<n;i++)
        {
            lefth[i]=max(lefth[i-1],height[i]);
        }
        for(int i=n-2;i>=0;i--)
        {
            righth[i]=max(righth[i+1],height[i]);
        }
        int sum=0;
        for(int i=0;i<n;i++)
        {
            sum+=(min(lefth[i],righth[i]))-height[i];
        }
        return sum;
    }
