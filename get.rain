```j
public class GetRain {
	  /*
	   * 给定 n 个非负整数表示每个宽度为 1 的柱子的高度图，计算按此排列的柱子，下雨之后能接多少雨水。
	   * 链接：https://leetcode-cn.com/problems/trapping-rain-water/
	   */
	  public static int trap(int[] height) {
	       int water = 0;
	     //  int left_max = 0,right_max =0;
	       int len = height.length;
	       int []left_max = new int[len];
	       int []right_max = new int[len];
	       left_max[0]=height[0];
	       for(int i=1;i<len;i++) 
	    	   left_max[i]=Math.max(left_max[i-1], height[i]);
	       right_max[len-1]=height[len-1];
	       for(int i=len-2;i>=0;i--) 
	    	   right_max[i]=Math.max(right_max[i+1], height[i]);
	       for(int i=0;i<len;i++) {
	    	  int level = Math.min( left_max[i],right_max[i]);
	    	   water+=level-height[i];
	       }
	    	return water;  
	   }

	public static void main(String[] args) {
		// TODO Auto-generated method stub
         int a[] = {2,0,2};
         System.out.println(trap(a));
	}

}
```
