class Solution {
public:
    bool uniqueOccurrences(vector<int>& arr) {
        sort(arr.begin(),arr.end());
        vector<int> arrcount;
        int n=arr.size();
        int count{1};

        for(int i=0;i<n-1;i++)
        {
            if(arr.at(i)==arr.at(i+1))
            {
                count++;
            }

            else{
                arrcount.push_back(count);
                count=1;
            }
        }

        arrcount.push_back(count);

        sort(arrcount.begin(),arrcount.end());

        for(int i=0;i<arrcount.size()-1;i++)
        {
            if(arrcount.at(i)==arrcount.at(i+1))
            return false;
        }

        return true;
    }
};
