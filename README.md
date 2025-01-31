public static void main(String args[])throws IOException {
        InputStreamReader r=new InputStreamReader(System.in);
        BufferedReader in=new BufferedReader(r);
        int n_test = Integer.parseInt(in.readLine());
        for (int i = 1; i <= n_test; i++) {
            String st = in.readLine();
            st = st.trim();
            st = st+' ';
            int nums[]=new int[3];
            String w="";
            int ind=0;
            for(int j=0;j<st.length();j++) {
                char ch = st.charAt(j);
                if (ch != ' ')
                    w += ch;
                else {
                    nums[ind] = Integer.parseInt(w);
                    ind += 1;
                    w = "";
                }
            }
        }
}









public static void main(String args[])throws IOException {
        InputStreamReader r=new InputStreamReader(System.in);
        BufferedReader in=new BufferedReader(r);
        int n_test = Integer.parseInt(in.readLine());
        for (int i = 1; i <= n_test; i++) {
            String st = in.readLine();
            st = st.trim();
            st = st+' ';
            int nums[]=new int[2];
            String w="";
            int ind=0;
            for(int j=0;j<st.length();j++) {
                char ch = st.charAt(j);
                if (ch != ' ')
                    w += ch;
                else {
                    nums[ind] = Integer.parseInt(w);
                    ind += 1;
                    w = "";
                }
            }
            int values[]=new int[nums[0]];
            ind=0;
            st=in.readLine();
            st = st.trim();
            st = st+' ';
            w="";
            for(int j=0;j<st.length();j++) {
                char ch = st.charAt(j);
                if (ch != ' ')
                    w += ch;
                else {
                    values[ind] = Integer.parseInt(w);
                    ind += 1;
                    w = "";
                }
            }
            check(nums[1], values);

        }
    }










    public static long[] prefixSum(int[] arr) {
            int n = arr.length;
            long[] prefixSum = new long[n];
    
            if (n > 0) {
                prefixSum[0] = arr[0];
                for (int i = 1; i < n; i++) {
                    prefixSum[i] = prefixSum[i - 1] + arr[i];
                }
            }
    
            return prefixSum;
        }
            public static int min(int[] arr) {
            if (arr == null || arr.length == 0) {
                throw new IllegalArgumentException("Array is empty or null");
            }
    
            int min = arr[0];  // Initialize with first element
            for (int i = 1; i < arr.length; i++) {
                if (arr[i] < min) {
                    min = arr[i];
                }
            }
            return min;
        }
        public static int max(int[] arr) {
            if (arr == null || arr.length == 0) {
                throw new IllegalArgumentException("Array is empty or null");
            }
    
            int max = arr[0];  // Initialize with first element
            for (int i = 1; i < arr.length; i++) {
                if (arr[i] > max) {
                    max = arr[i];
                }
            }
            return max;
        }
            public static long sum(int[] arr) {
            if (arr == null) {
                throw new IllegalArgumentException("Array is null");
            }
    
            long sum = 0; // Use long to avoid overflow
            for (int num : arr) {
                sum += num;
            }
            return sum;
        }
        public static void display2DArray(int[][] arr) {
            if (arr == null || arr.length == 0) {
                System.out.println("Array is empty or null");
                return;
            }
    
            for (int[] row : arr) {
                System.out.println(Arrays.toString(row));
            }
        }
    public static int[][] takeInput2DArray(BufferedReader br) throws IOException {
            // Read the first line and split it into row and column values
            String[] dimensions = br.readLine().split(" ");
            int rows = Integer.parseInt(dimensions[0]);
            int cols = Integer.parseInt(dimensions[1]);
    
            // Initialize the 2D array
            int[][] arr = new int[rows][cols];
    
            // Read the array row by row
            for (int i = 0; i < rows; i++) {
                String[] rowValues = br.readLine().split(" ");
                for (int j = 0; j < cols; j++) {
                    arr[i][j] = Integer.parseInt(rowValues[j]);
                }
            }
    
            return arr;
        }
                public static void printSDA(int [] arr){
                for(int v:arr){
                    System.out.print(v+" ");
                }
                System.out.println();
            }
            public static int countOdd(int[] arr){
                int c=0;
                for(int v:arr){
                    if(v%2!=0)c++;
                }
                return c;
            }
        public static int countEven(int[] arr){
            int c=0;
            for(int v:arr){
                if(v%2==0)c++;
            }
            return c;
        }
    public static void check(int value, int [] arr){
    
    }



    






