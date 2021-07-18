class Solution {
    public int[] plusOne(int[] digits) {
        int l=digits.length,rem=0,carry=0;
        int[] a=new int[l+1];
        a[0]=0;
        if(digits[l-1]<9)
        {
            digits[l-1]+=1;
            return digits;
        }
        if(digits[l-1]==9)
        {
            digits[l-1]+=1;
            rem=digits[l-1]%10;
            carry=digits[l-1]/10;
            digits[l-1]=rem;
        }
        for(int i=l-2;i>=0;i--)
        {
            if(carry==1)
            {
                digits[i]+=carry;
                carry=digits[i]/10;
                rem=digits[i]%10;
                digits[i]=rem;
            }
        }
        if(carry==0)
        {
            return digits;
        }
        else
        {
            for(int i=l-1;i>0;i--)
            {
                a[i]=digits[i];
            }
            if(carry==1)
                a[0]+=1;
            return a;
        }
       
    }
}
