Test1	   运行代码   
public class Test9 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int score[] = {25, 24, 12, 76, 101, 96,28};
		bubbleArray(score);
		printArray(score);
	}
	public static void printArray(int score[]) {
		for(int i = 0; i < score.length; i++) {
			 System.out.print(score[i] +" ");
		}
		System.out.println();
	}
	private static void bubbleArray(int[] score) {
		for(int i = 0;i < score.length - 1;i ++) {
			for(int j = 0;j < score.length - i -1; j++) {
				if(score[j] > score[j + 1]) {
					int temp = score[j];
					score[j] = score[j + 1];
					score[j + 1] = temp;
				}
			}
		}
	}
} 
     单元测试：
     
测试用例	测试步骤    预计输出                 实际输出
Test1	   运行代码   12 24 25 28 76 96 101    12 24 25 28 76 96 101

这个单元测试：
用到了  测试用例，测试步骤，预计输出，实际输出
	

